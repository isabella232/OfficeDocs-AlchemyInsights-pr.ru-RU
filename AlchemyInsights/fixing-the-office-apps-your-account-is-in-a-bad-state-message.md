---
title: Исправление Microsoft 365 приложений Ваша учетная запись находится в плохом сообщении состояния
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
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068249"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Исправление ошибки Microsoft 365 приложений "Ваша учетная запись находится в плохом состоянии"

Чтобы устранить эту ошибку, попробуйте следующие параметры на затронутом компьютере:

- Откройте Приложение Office, выберите **вход учетной** записи  >    >  **файла из всех учетных записей.** Снова войдите с помощью учетной записи пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очистка Office учетных](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) данных с Windows диспетчером учетных данных.<br>
  **Примечание:** Пути реестра за Office 2016 г. изменились до 16.0. Например, \Software\Microsoft\Office\16.0\Common\Identity\
- Если ошибка возникает при подключении к Office 365 с Office 2013 [г.,](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) включении современной проверки подлинности для Office клиента.

Дополнительные сведения см. в документе [How to troubleshoot non-browser apps that can't sign in to Microsoft 365, Azure, or Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

