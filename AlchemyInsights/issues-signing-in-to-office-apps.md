---
title: Проблемы с входом в Microsoft 365 приложения
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
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028053"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Исправление Microsoft 365 приложения "К сожалению, другая учетная запись организации уже подписана" сообщение

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

- Удалите все учетные записи, за исключением затрагиваемой учетной записи, Windows Параметры > **работу или школу.**
- [Очистка Office учетных](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) данных с Windows диспетчером учетных данных.<br/>
    **Примечание:** Пути реестра за Office 2016 г. изменились до 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Откройте Приложение Office, выберите **выход**  >    >  **учетной записи файла**. Затем впишитесь с помощью учетной записи пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Для компьютеров Mac см. статью [Не удается войти в приложение Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Дополнительные сведения см. в примере ["Извините,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)другая учетная запись организации уже подписана на этом компьютере" в Office .