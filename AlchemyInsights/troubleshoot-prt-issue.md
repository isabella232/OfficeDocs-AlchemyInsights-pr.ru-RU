---
title: Устранение неполадок с PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330972"
---
# <a name="troubleshoot-prt-issue"></a>Устранение неполадок с PRT

Чтобы любое устройство завершило проверку подлинности, оно должно быть полностью зарегистрировано и в хорошем состоянии и может приобретать маркер первичного обновления (PRT).

Гибридный процесс регистрации в Azure AD требует, чтобы устройства были в корпоративной сети. Он также работает над VPN, но есть некоторые оговорки к этому. Мы слышали, как клиенты, нуждающиеся в помощи в устранении неполадок в гибридном процессе регистрации в Azure AD, присоединяются к нему в условиях удаленной работы. Вот разбивка того, что происходит "под капотом" во время процесса регистрации.

**Среда облачной проверки подлинности (с помощью синхронизации и проверки подлинности паролей Azure AD)**

Этот поток регистрации также известен как "Sync Join".

1. Windows 10 записи SCP при входе пользователя на устройство.
    1. Устройство сначала пытается получить сведения клиента из клиентской SCP в реестре [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Дополнительные сведения см. в [этом документе](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. В случае сбой устройства взаимодействует с локальной службой Active Directory (AD), чтобы получить сведения о клиентах из точки подключения к службе (SCP). Чтобы проверить SCP, обратитесь к этому [документу.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Примечание.** Рекомендуется включить SCP в AD и использовать только клиентскую SCP для начальной проверки.

2. Windows 10 пытается связаться с Azure AD в системном контексте для проверки подлинности в отношении Azure AD. Вы можете проверить, может ли устройство получить доступ к ресурсам Майкрософт в учетной записи системы с помощью скрипта подключения к регистрации тестовых устройств.

3. Windows 10 создает самозаверяется сертификат и хранит его под объектом компьютера в локальной AD. Для этого требуется прямой доступ к контроллеру домена.

4. Объект устройства с сертификатом синхронизируется с Azure AD с помощью Azure AD Подключение. Цикл синхронизации по умолчанию составляет каждые 30 минут, но зависит от конфигурации azure AD Подключение. Дополнительные сведения можно получить в этом [документе.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. На этом этапе вы должны иметь возможность видеть объект в состоянии "Ожидающееся" в лезвии устройства портала Azure.

6. При следующем входе пользователя в Windows 10 регистрация будет завершена. 

**Примечание.** Если вы подключены к VPN, а процесс входа в систему входа завершает подключение к домену, можно запускать регистрацию вручную:
 1. Выдайте dsregcmd/join локально на запросе администратора или удаленно через PSExec на компьютер. Например, PsExec -s \\ win10client01 cmd, dsregcmd/join

 2. Дополнительные сведения о проблемах hybrid Join см. в материале [Проблема устройств устранения неполадок.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
