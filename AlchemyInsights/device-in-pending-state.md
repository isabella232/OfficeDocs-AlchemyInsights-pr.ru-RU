---
title: Устройство в ожидаемом состоянии
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914016"
---
# <a name="device-in-pending-state"></a>Устройство в ожидаемом состоянии

**Необходимые условия:**

1. Если вы впервые настраивали регистрации устройств, убедитесь, что вы рассмотрели введение в управление устройствами в [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) которое поможет вам получить устройства под управлением Azure AD.
2. Если вы непосредственно регистрируете устройства в Azure AD и регистрируете их в Intune, необходимо [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) убедиться, что вы настроили [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и сначала настроили лицензирование.
3. Убедитесь, что вы уполномочены выполнять операции в Azure AD и локальной AD. Только глобальный администратор Microsoft Azure AD может управлять параметрами регистрации устройств. Кроме того, для настройки автоматической регистрации в локальной службе Active Directory необходимы права администратора Active Directory и AD FS (если применимо).

Гибридный процесс регистрации в Azure AD требует, чтобы устройства были в корпоративной сети. Он также работает над VPN, но есть некоторые оговорки к этому. Мы слышали, как клиенты, нуждающиеся в помощи в устранении неполадок в гибридной регистрации Azure AD, присоединяются к процессу регистрации в удаленных условиях работы.

**Среда облачной проверки подлинности (с помощью синхронизации и проверки подлинности паролей Azure AD)**

Этот поток регистрации также известен как "Sync Join".

Вот разбивка того, что происходит во время процесса регистрации:

1. Windows 10 обнаруживает запись точки подключения к службе (SCP) при входе пользователя на устройство.

    1. Устройство сначала пытается получить сведения клиента из клиентской SCP в реестре [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Дополнительные сведения см. в [документе](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. В случае сбой устройства взаимодействует с локальной службой Active Directory для получения сведений о клиентах из SCP. Чтобы проверить SCP, обратитесь к этому [документу.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Рекомендуется включить SCP в Active Directory и использовать только клиентскую SCP для начальной проверки.

2. Windows 10 пытается связаться с Azure AD в системном контексте для проверки подлинности в отношении Azure AD.

    Вы можете проверить, может ли устройство получить доступ к ресурсам Microsoft в учетной записи системы с помощью скрипта подключения к регистрации [тестовых устройств.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 создает самозаверяется сертификат и хранит его под объектом компьютера в локальном Active Directory. Для этого требуется прямой доступ к контроллеру домена.

4. Объект устройства с сертификатом синхронизируется с Azure AD с помощью Azure AD Подключение. Цикл синхронизации по умолчанию составляет каждые 30 минут, но зависит от конфигурации Azure AD Подключение. Дополнительные сведения можно получить в этом [документе.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. На этом этапе вы сможете увидеть объект в состоянии **"Ожидание"** под лезвием устройства портала Azure.

6. При следующем входе пользователя в Windows 10 регистрация будет завершена.

    > [!NOTE]
    > Если вы подключены к VPN, а вход/вход прекращает подключение к домену, можно запускать регистрацию вручную. Для этого выполните следующие действия.
    >
    > Выдайте локальный запрос администратора или удаленно `dsregcmd /join` через PSExec на компьютер.
    >
    > Пример: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Общие проблемы с регистрацией Azure Active Directory см. в [faq Devices.](https://docs.microsoft.com/azure/active-directory/devices/faq)
