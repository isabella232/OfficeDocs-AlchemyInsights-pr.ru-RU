---
title: Параметры политики собраний
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376796"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="cd837-102">Управление политиками собраний в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cd837-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="cd837-103">Политики собраний используются для управления возможностями, доступными участникам собрания для собраний, запланированных пользователями в Организации.</span><span class="sxs-lookup"><span data-stu-id="cd837-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="cd837-104">Некоторые функции политик собраний могут не быть реализованы в центре администрирования Teams, но они помечаются как "скоро" в документации.</span><span class="sxs-lookup"><span data-stu-id="cd837-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="cd837-105">В этом случае, или если вы получаете сообщение об ошибке "не удается обновить политику, но повторите попытку позже" в центре администрирования Microsoft Teams, мы рекомендуем использовать PowerShell для создания или изменения политик собрания Teams.</span><span class="sxs-lookup"><span data-stu-id="cd837-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="cd837-106">Дополнительные сведения о политиках собраний содержатся в следующих ресурсах:</span><span class="sxs-lookup"><span data-stu-id="cd837-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="cd837-107">Чтобы узнать о создании политик, внесении изменений и назначении пользователям политики, ознакомьтесь со статьей [Управление политиками собраний в Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="cd837-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="cd837-108">Чтобы изменить политику с помощью командлетов PowerShell, ознакомьтесь с разделом [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="cd837-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="cd837-109">Необходимо использовать [модуль PowerShell Skype для бизнеса](https://www.microsoft.com/download/details.aspx?id=39366) для политик собраний Teams.</span><span class="sxs-lookup"><span data-stu-id="cd837-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="cd837-110">Ознакомьтесь с [документацией по командлетам \* – кстеамсмитингполици](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="cd837-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="cd837-111">**Примечание:** Для вступления в силу изменений политики для пользователей может потребоваться до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="cd837-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="cd837-112">Возможно, вы не сможете вносить изменения сразу для вновь созданных политик; Подождите 4 часа и попытайтесь изменить вновь созданную политику.</span><span class="sxs-lookup"><span data-stu-id="cd837-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="cd837-113">Если у вас по-прежнему возникают проблемы, попробуйте использовать PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd837-113">If you're still having problems, try PowerShell.</span></span>  