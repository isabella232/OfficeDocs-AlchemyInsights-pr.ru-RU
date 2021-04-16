---
title: Исправление приложений Microsoft 365 Ваша учетная запись находится в плохом состоянии сообщения
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
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812549"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Исправление ошибки приложений Microsoft 365 "Ваша учетная запись находится в плохом состоянии"

Чтобы устранить эту ошибку, попробуйте следующие параметры на затронутом компьютере:

- Откройте приложение Office, выберите **вход учетной** записи  >    >  **файла из всех учетных записей.** Снова войдите с помощью учетной записи пользователя с действительной лицензией. Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.<br>
  **Примечание:** Пути реестра Office 2016 изменились до 16.0. Например, \Software\Microsoft\Office\16.0\Common\Identity\
- Если ошибка возникает при подключении к Office 365 с [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) помощью Office 2013, включении современной проверки подлинности для клиента Office.

Дополнительные сведения см. в документе [How to troubleshoot non-browser apps that can't sign in to Microsoft 365, Azure, or Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

