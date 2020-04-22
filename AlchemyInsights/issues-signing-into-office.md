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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763014"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="6e902-102">Проблемы с входом в приложения Office</span><span class="sxs-lookup"><span data-stu-id="6e902-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="6e902-103">Чтобы устранить проблемы с входом в приложения Office, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="6e902-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="6e902-104">Удалите все рабочие учетные записи, кроме затронутой учетной записи, используя параметры Windows > **доступ к работе или учебным заведениям**.</span><span class="sxs-lookup"><span data-stu-id="6e902-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="6e902-105">[Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="6e902-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6e902-106">**Примечание:** Пути реестра для Office 2016 изменились на 16,0.</span><span class="sxs-lookup"><span data-stu-id="6e902-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6e902-107">(Пример: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6e902-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="6e902-108">Откройте приложение Office, выберите пункт**выход из\*\*\*\*учетной записи** >  **файла** > . Войдите в систему, используя учетную запись пользователя с действительной лицензией.</span><span class="sxs-lookup"><span data-stu-id="6e902-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="6e902-109">Подробные сведения см. в статье [Учетные записи в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="6e902-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="6e902-110">Для компьютеров Mac см. статью [Не удается войти в приложение Office 2016 для Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="6e902-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="6e902-111">Если ошибки возникают при подключении к Microsoft 365 с помощью Office 2013, включите для клиента Office современная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="6e902-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="6e902-112">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="6e902-112">For more information, see:</span></span>
- [<span data-ttu-id="6e902-113">Вы не можете войти в Microsoft 365, Azure или Intune.</span><span class="sxs-lookup"><span data-stu-id="6e902-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="6e902-114">Проблемы с подключением при входе после обновления до Office 2016 сборка 16.0.7967 в Windows 10</span><span class="sxs-lookup"><span data-stu-id="6e902-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="6e902-115">"К сожалению, в Office уже выполнен вход с другой учетной записью из вашей организации" в Office</span><span class="sxs-lookup"><span data-stu-id="6e902-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="6e902-116">Устранение проблем с входом в систему Office современная проверка подлинности при использовании ADFS</span><span class="sxs-lookup"><span data-stu-id="6e902-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)