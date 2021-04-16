---
title: Не удается активировать Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812585"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="8ebdf-102">Не удается активировать Office</span><span class="sxs-lookup"><span data-stu-id="8ebdf-102">Unable to activate Office</span></span>

- <span data-ttu-id="8ebdf-103">Проверьте, не истек ли срок действия вашей подписки.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="8ebdf-104">Убедитесь в наличии подписки, поддерживающей клиентские лицензии, например Office 365 бизнес или бизнес премиум, и [убедитесь, что пользователю назначена лицензия](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8ebdf-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="8ebdf-105">Убедитесь, что пользователь входит в Office с учетной записью, которой назначена лицензия.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="8ebdf-106">Проверьте [страницу работоспособности службы Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) на наличие известных проблем в службе.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="8ebdf-107">Проверьте параметры брандмауэра, антивирусной программы и прокси-сервера, чтобы убедиться, что они не блокируют доступ приложений Microsoft 365 к Интернету.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="8ebdf-108">См. статью [URL-адреса и диапазоны IP-адресов Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-адреса и диапазоны IP-адресов Office 365").</span><span class="sxs-lookup"><span data-stu-id="8ebdf-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="8ebdf-109">**Совет**: на компьютерах с Windows можно диагностировать и автоматически устранять некоторые распространенные проблемы с входом в Office.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8ebdf-110">Для использования нашего автоматического инструмента скачайте и запустите **[Помощник по поддержке и восстановлению Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8ebdf-111">Воспользуйтесь следующими инструкциями по устранению неполадок:</span><span class="sxs-lookup"><span data-stu-id="8ebdf-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="8ebdf-112">Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="8ebdf-113">[Удалите](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) и [заново назначьте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) лицензию на Office, а затем [войти в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью затронутой учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ebdf-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="8ebdf-114">Запустите [средство устранения неполадок активации](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="8ebdf-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="8ebdf-115">Сбросьте состояние активации Office</span><span class="sxs-lookup"><span data-stu-id="8ebdf-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Сбросьте состояние активации Office")
- [<span data-ttu-id="8ebdf-116">Запустите восстановление Office по сети</span><span class="sxs-lookup"><span data-stu-id="8ebdf-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="8ebdf-117">Дополнительные решения по устранению неполадок см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="8ebdf-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="8ebdf-118">Ошибки, связанные с нелицензированным продуктом и активацией Office</span><span class="sxs-lookup"><span data-stu-id="8ebdf-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="8ebdf-119">Ошибка "Не удается подключиться к вашей учетной записи. Повторите попытку позже" при активации Office</span><span class="sxs-lookup"><span data-stu-id="8ebdf-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)