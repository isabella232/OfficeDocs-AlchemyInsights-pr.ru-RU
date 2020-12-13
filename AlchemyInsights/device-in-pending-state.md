---
title: Устройство находится в состоянии ожидания
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652244"
---
# <a name="device-in-pending-state"></a>Устройство находится в состоянии ожидания

**Необходимые условия:**

1. Если вы настраивали регистрацию устройств в первый раз, убедитесь, что вы рассмотрели введение в управление устройствами в [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) которое поможет вам получить устройства под управлением Azure AD.
2. Если вы регистрируете устройства непосредственно в Azure AD и регистрируете их в Intune, вам [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) необходимо убедиться, что вы настроили [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и сначала настроили лицензирование.
3. Убедитесь, что вы уполномочены выполнять операции в Azure AD и локальной службе AD. Только глобальный администратор в Azure AD может управлять настройками регистрации устройств. Кроме того, при настройке автоматической регистрации в локальной службе Active Directory необходимо быть администратором Active Directory и AD FS (если это возможно).

Для регистрации гибридного присоединить Azure AD устройства должны быть в корпоративной сети. Она также работает по VPN, но есть некоторые оговорки. Мы узнали, что клиентам нужна помощь по устранению неполадок при регистрации гибридного присоединиться к Azure AD в условиях удаленной работы.

**Облачная среда проверки подлинности (с помощью синхронизации и сквозной проверки подлинности паролей Azure AD)**

Этот процесс регистрации также называется "Sync Join".

Вот разбивка того, что происходит во время регистрации:

1. Windows 10 обнаруживает запись точки подключения службы (SCP) при входе пользователя на устройство.

    1. Устройство сначала пытается получить сведения о клиенте из клиентского SCP в реестре [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Дополнительные сведения см. в [документе.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Если происходит сбой, устройство взаимодействует с локальной службой Active Directory для получения сведений о клиенте из SCP. Чтобы проверить SCP, обратитесь к этому [документу.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Для начальной проверки рекомендуется включить SCP в Active Directory и использовать только клиентский SCP.

2. Windows 10 пытается связаться с Azure AD в контексте системы для проверки подлинности в Azure AD.

    Вы можете проверить, может ли устройство получить доступ к ресурсам Майкрософт в системной учетной записи с помощью скрипта подключения для регистрации [тестовых устройств.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 создает самозаверяяя сертификат и сохраняет его под объектом компьютера в локальной службе Active Directory. Для этого требуется прямой просмотр контроллера домена.

4. Объект устройства с сертификатом синхронизируется с Azure AD через Azure AD Connect. По умолчанию цикл синхронизации каждые 30 минут, но он зависит от конфигурации Azure AD Connect. Дополнительные сведения можно получить в этом [документе.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. На этом этапе вы сможете увидеть устройствотемы в состоянии "Ожидание" в blade устройства портала Azure.

6. При следующем входе пользователя в Windows 10 регистрация будет завершена.

    > [!NOTE]
    > Если вы подключены к VPN и при входе или входе в систему подключение к домену прерывается, регистрацию можно запускать вручную. Для этого выполните следующие действия.
    >
    > `dsregcmd /join`Выдайте локальное запрос администратора или удаленно через PSExec на компьютере.
    >
    > Пример: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Распространенные проблемы с регистрацией устройств Azure Active Directory см. в часто [задаваемом вопросе о устройствах.](https://docs.microsoft.com/azure/active-directory/devices/faq)
