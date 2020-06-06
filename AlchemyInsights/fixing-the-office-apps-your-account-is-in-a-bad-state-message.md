---
title: Устранение неполадок в приложениях Microsoft 365, которые ваша учетная запись находится в ошибочном сообщении о состоянии
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
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580130"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Исправление ошибки в приложениях Microsoft 365 "Ваша учетная запись находится в неправильном состоянии"

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия на затронутом компьютере:

- Откройте приложение Office, выберите пункт **File**  >  выйти из**учетной записи**файла  >  **выход из всех учетных записей**. Снова войдите с помощью учетной записи пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br>
  **Примечание:** Пути реестра для Office 2016 изменились на 16,0. Например, \Software\Microsoft\Office\16.0\Common\Identity\
- Если ошибка возникает при подключении к Office 365 с помощью Office 2013, [включите современная проверка подлинности](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) для клиента Office.

Дополнительные сведения см. [Устранение неполадок в приложениях, не являющихся браузерами, которые не могут войти в Microsoft 365, Azure или Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

