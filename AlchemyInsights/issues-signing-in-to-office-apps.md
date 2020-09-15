---
title: Проблемы с входом в приложения Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695336"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Устранение неполадок в приложениях Microsoft 365: "сообщение уже подписано другой учетной записью в организации"

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

- Удалите все рабочие учетные записи, кроме затронутой учетной записи, используя параметры Windows > **доступ к работе или учебным заведениям**.
- [Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br/>
    **Примечание:** Пути реестра для Office 2016 изменились на 16,0. (Пример: \Software\Microsoft\Office\16.0\Common\Identity\)
- Откройте приложение Office, выберите пункт **File**  >  выход из**учетной записи**файла  >  **Sign Out**. Войдите в систему, используя учетную запись пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Для компьютеров Mac см. статью [Не удается войти в приложение Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Дополнительные сведения см. [в разделе "к сожалению, на этом компьютере уже выполнен вход в систему с другой учетной записью" в Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).