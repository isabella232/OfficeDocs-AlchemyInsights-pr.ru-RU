---
title: Проблемы с входом в приложения Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833088"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Исправление приложений Microsoft 365 "К сожалению, другая учетная запись из организации уже подписана" сообщение

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

- Удалите все учетные записи, за исключением затронутой учетной записи, с помощью параметров Windows > **работы или учебного заведения.**
- [Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.<br/>
    **Примечание:** Пути реестра Office 2016 изменились до 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Откройте приложение Office, выберите **выход учетной**  >    >  **записи файла**. Затем впишитесь с помощью учетной записи пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Для компьютеров Mac см. статью [Не удается войти в приложение Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Дополнительные сведения см. в [примере "Извините,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)другая учетная запись организации уже подписана на этом компьютере" в Office.