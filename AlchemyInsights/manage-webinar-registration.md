---
title: Управление регистрацией в вебинаре
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783143"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="f9eeb-102">Управление регистрацией в вебинаре</span><span class="sxs-lookup"><span data-stu-id="f9eeb-102">Manage webinar registration</span></span>

<span data-ttu-id="f9eeb-103">Управляйте тем, кто может регистрироваться в вебинарах Teams, с помощью команд PowerShell Teams.</span><span class="sxs-lookup"><span data-stu-id="f9eeb-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="f9eeb-104">Сведения об установке PowerShell Teams см. в разделе [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="f9eeb-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="f9eeb-105">По умолчанию параметр *whoCanRegister* включен и ему присвоено значение **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="f9eeb-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="f9eeb-106">Чтобы разрешить регистрацию всем, в том числе анонимным пользователям, присвойте политике собраний значение **Все** с помощью команды PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f9eeb-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="f9eeb-107">**Примечание**. Если анонимное присоединение отключено в параметрах собрания, анонимные пользователи не смогут присоединяться к вебинарам.</span><span class="sxs-lookup"><span data-stu-id="f9eeb-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="f9eeb-108">Дополнительные сведения и инструкции по включению этого параметра см. в статье [Управление параметрами собраний в Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="f9eeb-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="f9eeb-109">Если вы хотите отключить регистрацию в собраниях, присвойте параметру *allowMeetingRegistration* значение **False**.</span><span class="sxs-lookup"><span data-stu-id="f9eeb-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="f9eeb-110">Дополнительные сведения о настройке того, кто может регистрироваться в вебинарах, см. в разделе [Настройка пользователей, которые могут регистрироваться в вебинарах](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="f9eeb-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="f9eeb-111">Дополнительные сведения о параметрах Microsoft Списки см. в статье [Управление параметрами для Microsoft Списки](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="f9eeb-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
