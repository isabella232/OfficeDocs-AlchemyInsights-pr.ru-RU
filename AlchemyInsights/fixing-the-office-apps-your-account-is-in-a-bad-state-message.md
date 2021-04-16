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
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="9a1a6-102">Исправление ошибки приложений Microsoft 365 "Ваша учетная запись находится в плохом состоянии"</span><span class="sxs-lookup"><span data-stu-id="9a1a6-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="9a1a6-103">Чтобы устранить эту ошибку, попробуйте следующие параметры на затронутом компьютере:</span><span class="sxs-lookup"><span data-stu-id="9a1a6-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="9a1a6-104">Откройте приложение Office, выберите **вход учетной** записи  >    >  **файла из всех учетных записей.**</span><span class="sxs-lookup"><span data-stu-id="9a1a6-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="9a1a6-105">Снова войдите с помощью учетной записи пользователя с действительной лицензией.</span><span class="sxs-lookup"><span data-stu-id="9a1a6-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="9a1a6-106">Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="9a1a6-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="9a1a6-107">[Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="9a1a6-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="9a1a6-108">**Примечание:** Пути реестра Office 2016 изменились до 16.0.</span><span class="sxs-lookup"><span data-stu-id="9a1a6-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9a1a6-109">Например, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="9a1a6-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="9a1a6-110">Если ошибка возникает при подключении к Office 365 с [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) помощью Office 2013, включении современной проверки подлинности для клиента Office.</span><span class="sxs-lookup"><span data-stu-id="9a1a6-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="9a1a6-111">Дополнительные сведения см. в документе [How to troubleshoot non-browser apps that can't sign in to Microsoft 365, Azure, or Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="9a1a6-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

