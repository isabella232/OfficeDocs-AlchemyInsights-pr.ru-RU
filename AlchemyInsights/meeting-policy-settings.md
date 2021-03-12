---
title: Параметры политики собраний
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704619"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="08705-102">Управление политиками собраний в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="08705-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="08705-103">**Примечание. Изменение политики для пользователей может занять до 24 часов.**</span><span class="sxs-lookup"><span data-stu-id="08705-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="08705-104">Возможно, вы не сможете немедленно внести изменения в вновь созданные политики; подождите 4 часа и снова попытайтесь изменить вновь созданную политику.</span><span class="sxs-lookup"><span data-stu-id="08705-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="08705-105">Политики собраний используются для управления функциями, доступными участникам собраний для собраний, запланированных пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="08705-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="08705-106">Некоторые функции политик собраний пока не могут быть реализованы в центре администрирования Teams (они помечены как "скоро" в документации).</span><span class="sxs-lookup"><span data-stu-id="08705-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="08705-107">В этом случае или при получении ошибки типа "Мы не можем обновить политику прямо сейчас, но попробуйте ее еще раз" в центре администрирования Microsoft Teams, рекомендуется использовать PowerShell для создания или изменения политик собраний Teams.</span><span class="sxs-lookup"><span data-stu-id="08705-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="08705-108">Дополнительные сведения о политиках собраний см. в следующих ресурсах:</span><span class="sxs-lookup"><span data-stu-id="08705-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="08705-109">Чтобы узнать о создании политик, внесении изменений и назначении пользователей политике, см. в руб. Управление политиками [собраний в Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="08705-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="08705-110">Чтобы изменить политику с помощью командлетов PowerShell, см. в обзоре [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="08705-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="08705-111">Для политик собраний Teams необходимо использовать модуль Skype для бизнеса [PowerShell.](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector)</span><span class="sxs-lookup"><span data-stu-id="08705-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="08705-112">Дополнительные сведения см. в документации по [cmdlets \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="08705-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

