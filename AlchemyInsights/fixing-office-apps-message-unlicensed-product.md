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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798693"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="45478-102">Не удается активировать Office</span><span class="sxs-lookup"><span data-stu-id="45478-102">Unable to activate Office</span></span>

<span data-ttu-id="45478-103">**Примечание**. Если вы используете более старую версию Windows (например, Windows 7), по умолчанию включите протокол TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="45478-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="45478-104">Дополнительные сведения см. в статье [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="45478-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="45478-105">Проверьте, не истек ли срок действия вашей подписки.</span><span class="sxs-lookup"><span data-stu-id="45478-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="45478-106">Убедитесь в наличии подписки, поддерживающей клиентские лицензии, например Office 365 бизнес или бизнес премиум, и [убедитесь, что пользователю назначена лицензия](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="45478-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="45478-107">Убедитесь, что пользователь входит в Office с учетной записью, которой назначена лицензия.</span><span class="sxs-lookup"><span data-stu-id="45478-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="45478-108">Проверьте [страницу работоспособности службы Office 365](/office365/enterprise/view-service-health) на наличие известных проблем в службе.</span><span class="sxs-lookup"><span data-stu-id="45478-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="45478-p102">Проверьте параметры брандмауэра, антивирусной программы и прокси-сервера, чтобы убедиться, что они не блокируют доступ приложений Microsoft 365 к Интернету. См. статью [URL-адреса и диапазоны IP-адресов Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL-адреса и диапазоны IP-адресов Office 365").</span><span class="sxs-lookup"><span data-stu-id="45478-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="45478-111">**Совет**: на компьютерах с Windows можно диагностировать и автоматически устранять некоторые распространенные проблемы с входом в Office.</span><span class="sxs-lookup"><span data-stu-id="45478-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="45478-112">Для использования нашего автоматического инструмента скачайте и запустите **[Помощник по поддержке и восстановлению Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="45478-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="45478-113">Воспользуйтесь следующими инструкциями по устранению неполадок:</span><span class="sxs-lookup"><span data-stu-id="45478-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="45478-114">Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="45478-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="45478-115">[Удалите](/microsoft-365/admin/manage/remove-licenses-from-users) и [заново назначьте](/microsoft-365/admin/manage/assign-licenses-to-users) лицензию на Office, а затем [войти в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью затронутой учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="45478-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="45478-116">Запустите [средство устранения неполадок активации](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="45478-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="45478-117">Сбросьте состояние активации Office</span><span class="sxs-lookup"><span data-stu-id="45478-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Сбросьте состояние активации Office")
- [<span data-ttu-id="45478-118">Запустите восстановление Office по сети</span><span class="sxs-lookup"><span data-stu-id="45478-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="45478-119">Дополнительные решения по устранению неполадок см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="45478-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="45478-120">Ошибки, связанные с нелицензированным продуктом и активацией Office</span><span class="sxs-lookup"><span data-stu-id="45478-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="45478-121">Ошибка "Не удается подключиться к вашей учетной записи. Повторите попытку позже" при активации Office</span><span class="sxs-lookup"><span data-stu-id="45478-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)