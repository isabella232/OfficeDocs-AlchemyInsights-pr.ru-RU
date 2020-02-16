---
title: Исправление приложений Office, в которых ваша учетная запись находится в ошибочном сообщении о состоянии
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969737"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Исправление ошибки приложений Office "Ваша учетная запись находится в неправильном состоянии"

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия на затронутом компьютере:

- Откройте приложение Office, выберите пункт выйти из**учетной записи** >  **файла** > **выход из всех учетных записей**. Повторно выполните вход, используя учетную запись пользователя с действительной лицензией. Более подробную информацию можно узнать [в статье Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br>
  **Примечание:** Пути реестра для Office 2016 изменились на 16,0. Например, \Software\Microsoft\Office\16.0\Common\Identity\
- На затронутом компьютере установите параметр Енаблеадал = 0, выполнив следующие действия:  
     1. Щелкните правой кнопкой мыши кнопку Windows и выберите команду **выполнить**. В поле **Открыть** введите **regedit**и нажмите кнопку **ОК**.
     2. Выберите **Да** , если будет предложено разрешить редактору реестра вносить изменения на устройстве.
    3. В редакторе реестра добавьте значение DWORD Енаблеадал с параметром 0 в раздел HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Если ошибка возникает при подключении к Office 365 с помощью Office 2013, [включите современная проверка подлинности](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) для клиента Office.

Дополнительные сведения см. [Устранение неполадок в приложениях, не являющихся браузерами, которые не могут войти в Office 365, Azure или Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

