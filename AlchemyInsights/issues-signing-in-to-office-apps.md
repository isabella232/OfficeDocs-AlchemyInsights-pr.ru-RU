---
title: Проблемы с входом в приложения Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938317"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="4ff7d-102">Устранение неполадок в приложениях Office: "сообщение уже подписано другой учетной записью из вашей организации"</span><span class="sxs-lookup"><span data-stu-id="4ff7d-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="4ff7d-103">Чтобы устранить эту ошибку, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="4ff7d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="4ff7d-104">Удалите все рабочие учетные записи, кроме затронутой учетной записи, используя параметры Windows > **доступ к работе или учебным**заведениям.</span><span class="sxs-lookup"><span data-stu-id="4ff7d-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="4ff7d-105">[Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="4ff7d-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="4ff7d-106">**Примечание:** Пути реестра для Office 2016 изменились на 16,0.</span><span class="sxs-lookup"><span data-stu-id="4ff7d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="4ff7d-107">(Пример: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="4ff7d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="4ff7d-108">Откройте приложение Office, выберите пункт**выход из\*\*\*\*учетной записи** >  **файла** > . Войдите в систему, используя учетную запись пользователя с действительной лицензией.</span><span class="sxs-lookup"><span data-stu-id="4ff7d-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="4ff7d-109">Более подробную информацию можно узнать [в статье Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="4ff7d-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="4ff7d-110">В разделе Mac [не удается войти в приложение Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="4ff7d-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="4ff7d-111">Дополнительные сведения см. [в разделе "к сожалению, на этом компьютере уже выполнен вход в систему с другой учетной записью" в Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="4ff7d-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>