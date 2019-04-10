---
title: Совместное использование с внешними пользователями не работает
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747611"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="fc9dd-102">Устранение неполадок при совместном использовании контента SharePoint с внешними пользователями</span><span class="sxs-lookup"><span data-stu-id="fc9dd-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="fc9dd-103">Убедитесь, что для вашей организации включен внешний общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="fc9dd-104">Перейдите на [страницу " &amp; надстройки служб" в центре администрирования Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)и нажмите кнопку **сайты**.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="fc9dd-105">Убедитесь, что параметр включен.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="fc9dd-106">Если выбран параметр "только существующие внешние пользователи", убедитесь, что внешний пользователь указан в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="fc9dd-107">Убедитесь, что для сайта включен внешний общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="fc9dd-108">Для классического семейства веб-сайтов:</span><span class="sxs-lookup"><span data-stu-id="fc9dd-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="fc9dd-109">В разделе новый центр администрирования SharePoint в левой области щелкните **сайты**.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="fc9dd-110">Выберите сайт или сайты, а затем на ленте щелкните **общий доступ**.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="fc9dd-111">Для сайта группы, принадлежащего к группе Office 365 или сайту для общения:</span><span class="sxs-lookup"><span data-stu-id="fc9dd-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="fc9dd-112">Эти новые типы сайтов имеют те же параметры общего доступа, что и настройка всей Организации, за исключением случаев, когда настройка уровня организации позволяет предоставлять общий доступ к файлам с помощью ссылок, не требующих входа в систему.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="fc9dd-113">В этом случае сайты разрешают общий доступ новым и существующим внешним пользователям, которые входят в систему.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="fc9dd-114">Чтобы изменить параметр для определенных сайтов, используйте новый центр администрирования SharePoint или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="fc9dd-115">[Дополнительные сведения](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="fc9dd-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="fc9dd-116">Настройка внешнего общего доступа для любого сайта может быть более строгой, чем настройка на уровне Организации, но не более, чем значение параметра для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="fc9dd-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

