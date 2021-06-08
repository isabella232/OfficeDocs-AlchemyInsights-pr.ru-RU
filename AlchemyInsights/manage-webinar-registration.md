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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798657"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="6fc78-102">Управление регистрацией в вебинаре</span><span class="sxs-lookup"><span data-stu-id="6fc78-102">Manage webinar registration</span></span>

<span data-ttu-id="6fc78-103">Управляйте тем, кто может регистрироваться в вебинарах Teams, с помощью команд PowerShell Teams.</span><span class="sxs-lookup"><span data-stu-id="6fc78-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="6fc78-104">Сведения об установке PowerShell Teams см. в разделе [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="6fc78-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="6fc78-105">По умолчанию параметр *whoCanRegister* включен и ему присвоено значение **Все**.</span><span class="sxs-lookup"><span data-stu-id="6fc78-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="6fc78-106">Если в приглашении на собрание вы не видите параметр, разрешающий регистрацию для всех пользователей, повторно запустите параметр *WhoCanRegister* со значением "Все" и подождите 24 часа.</span><span class="sxs-lookup"><span data-stu-id="6fc78-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="6fc78-107">Чтобы повторно запустить параметр *WhoCanRegister*, используйте команду Powershell:</span><span class="sxs-lookup"><span data-stu-id="6fc78-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="6fc78-108">**Примечание**. Если анонимное присоединение отключено в параметрах собрания, анонимные пользователи не смогут присоединяться к вебинарам.</span><span class="sxs-lookup"><span data-stu-id="6fc78-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="6fc78-109">Дополнительные сведения и инструкции по включению этого параметра см. в статье [Управление параметрами собраний в Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6fc78-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="6fc78-110">Если вы хотите отключить регистрацию в собраниях, присвойте параметру *allowMeetingRegistration* значение **False**.</span><span class="sxs-lookup"><span data-stu-id="6fc78-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="6fc78-111">Дополнительные сведения о настройке того, кто может регистрироваться в вебинарах, см. в разделе [Настройка пользователей, которые могут регистрироваться в вебинарах](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="6fc78-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="6fc78-112">Дополнительные сведения о параметрах Microsoft Списки см. в статье [Управление параметрами для Microsoft Списки](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="6fc78-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
