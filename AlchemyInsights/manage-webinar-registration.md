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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760849"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="82ce2-102">Управление регистрацией в вебинаре</span><span class="sxs-lookup"><span data-stu-id="82ce2-102">Manage webinar registration</span></span>

<span data-ttu-id="82ce2-103">С помощью команд PowerShell Teams вы можете управлять тем, кто может регистрироваться в вебинарах Teams.</span><span class="sxs-lookup"><span data-stu-id="82ce2-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="82ce2-104">По умолчанию параметр *whoCanRegister* включен и ему присвоено значение **Все**.</span><span class="sxs-lookup"><span data-stu-id="82ce2-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="82ce2-105">Если вы хотите отключить регистрацию в собраниях, присвойте параметру *allowMeetingRegistration* значение **False**.</span><span class="sxs-lookup"><span data-stu-id="82ce2-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="82ce2-106">Чтобы изменить эти параметры, установите [PowerShell Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="82ce2-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="82ce2-107">Кроме того, к вебинарам Teams применяются политики собраний.</span><span class="sxs-lookup"><span data-stu-id="82ce2-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="82ce2-108">Например, если анонимное присоединение отключено в параметрах собрания, анонимные пользователи не смогут присоединяться к вебинарам.</span><span class="sxs-lookup"><span data-stu-id="82ce2-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="82ce2-109">Дополнительные сведения о настройке того, кто может регистрироваться в вебинарах, см. в разделе [Настройка пользователей, которые могут регистрироваться в вебинарах](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="82ce2-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="82ce2-110">Дополнительные сведения о параметрах Microsoft Списки см. в статье [Управление параметрами для Microsoft Списки](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="82ce2-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>