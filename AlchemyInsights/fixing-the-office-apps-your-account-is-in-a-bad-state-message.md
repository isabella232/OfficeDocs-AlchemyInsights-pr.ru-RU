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
ms.openlocfilehash: b28865ff1da434a254c9051183074be35cdd0252
ms.sourcegitcommit: 9b2b162ad651e2c3d9d0c746f67a78334592f076
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2020
ms.locfileid: "43547975"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Исправление ошибки приложений Office "Ваша учетная запись находится в неправильном состоянии"

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия на затронутом компьютере:

- Откройте приложение Office, выберите пункт выйти из**учетной записи** >  **файла** > **выход из всех учетных записей**. Повторно выполните вход, используя учетную запись пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.<br>
  **Примечание:** Пути реестра для Office 2016 изменились на 16,0. Например, \Software\Microsoft\Office\16.0\Common\Identity\
- Если ошибка возникает при подключении к Office 365 с помощью Office 2013, [включите современная проверка подлинности](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) для клиента Office.

Дополнительные сведения см. [Устранение неполадок в приложениях, не являющихся браузерами, которые не могут войти в Office 365, Azure или Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

