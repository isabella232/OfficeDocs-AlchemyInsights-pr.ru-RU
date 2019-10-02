---
title: Удаление или исключение Teams из установок Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37344250"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="b7891-102">Удаление или исключение команд из новых или существующих установок Office</span><span class="sxs-lookup"><span data-stu-id="b7891-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="b7891-103">Microsoft Teams теперь входит в состав Office 365 профессиональный плюс, Office 365 для бизнеса и Office для Mac.</span><span class="sxs-lookup"><span data-stu-id="b7891-103">Microsoft Teams is now included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="b7891-104">Используйте [средство развертывания Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) , чтобы исключить команды из новых установок Office.</span><span class="sxs-lookup"><span data-stu-id="b7891-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="b7891-105">Чтобы *Удалить* Teams с устройства под управлением Windows, ознакомьтесь с разделом [uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="b7891-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="b7891-106">Чтобы очистить Microsoft Teams с нескольких целевых компьютеров или пользователей, ознакомьтесь со статьей " [Очистка развертывания Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)".</span><span class="sxs-lookup"><span data-stu-id="b7891-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="b7891-107">Используйте параметр [превенттеамсинсталл](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , чтобы запретить Microsoft Teams автоматически устанавливать Office.</span><span class="sxs-lookup"><span data-stu-id="b7891-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="b7891-108">Используйте параметр [превентфирстлаунчафтеринсталл](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *до установки Teams*, чтобы предотвратить автоматический запуск Microsoft Teams после установки.</span><span class="sxs-lookup"><span data-stu-id="b7891-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="b7891-109">Если вы используете Office для Mac, ознакомьтесь с разделом [Установка Microsoft Teams на компьютере Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="b7891-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>