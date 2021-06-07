---
title: Включение вебинаров Teams
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760857"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="5a308-102">Включение вебинаров Teams</span><span class="sxs-lookup"><span data-stu-id="5a308-102">Enable Teams Webinars</span></span>

<span data-ttu-id="5a308-103">Вебинары включены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5a308-103">Webinars are enabled by default.</span></span> <span data-ttu-id="5a308-104">С помощью команд PowerShell Teams вы можете управлять тем, кто может планировать вебинары Teams и регистрироваться в них.</span><span class="sxs-lookup"><span data-stu-id="5a308-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="5a308-105">Все пользователи, которые могут создавать собрания, также могут создавать вебинары.</span><span class="sxs-lookup"><span data-stu-id="5a308-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="5a308-106">Если вы хотите управлять тем, кто может планировать вебинары Teams, используйте параметр *allowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="5a308-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="5a308-107">По умолчанию параметр *whoCanRegister* включен и ему присвоено значение **Все**.</span><span class="sxs-lookup"><span data-stu-id="5a308-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="5a308-108">Если вы хотите отключить регистрацию в собраниях, присвойте параметру *allowMeetingRegistration* значение **False**.</span><span class="sxs-lookup"><span data-stu-id="5a308-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="5a308-109">Чтобы изменить эти параметры, установите [PowerShell Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="5a308-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="5a308-110">Кроме того, к вебинарам Teams применяются политики собраний.</span><span class="sxs-lookup"><span data-stu-id="5a308-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="5a308-111">Например, если анонимное присоединение отключено в параметрах собрания, анонимные пользователи не смогут присоединяться к вебинарам.</span><span class="sxs-lookup"><span data-stu-id="5a308-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="5a308-112">Дополнительные сведения о настройке того, кто может регистрироваться в вебинарах, см. в разделе [Настройка пользователей, которые могут регистрироваться в вебинарах](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="5a308-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="5a308-113">Дополнительные сведения о параметрах Microsoft Списки см. в статье [Управление параметрами для Microsoft Списки](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="5a308-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>