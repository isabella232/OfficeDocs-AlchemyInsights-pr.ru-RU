---
title: Общий доступ для внешних пользователей не работает
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308697"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="408ad-102">Устранение неполадок, общий доступ к содержимому SharePoint с внешними пользователями</span><span class="sxs-lookup"><span data-stu-id="408ad-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="408ad-103">Убедитесь в том, что внешний общий доступ включен для вашей организации:</span><span class="sxs-lookup"><span data-stu-id="408ad-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="408ad-104">Последовательно выберите пункты [служб &amp; страницы надстроек в центре администрирования Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)и нажмите кнопку **узлы**.</span><span class="sxs-lookup"><span data-stu-id="408ad-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="408ad-p101">Убедитесь в том, что включен параметр «ON». Если выбран «Только существующие внешние пользователи», убедитесь, что внешний пользователь указан в центре администрирования Office 365.</span><span class="sxs-lookup"><span data-stu-id="408ad-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="408ad-p102">Убедитесь, что внешний общий доступ к ней для сайта. Для семейства сайтов классический:</span><span class="sxs-lookup"><span data-stu-id="408ad-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="408ad-109">В классический центра администрирования SharePoint в области слева щелкните **семейств веб-сайтов**.</span><span class="sxs-lookup"><span data-stu-id="408ad-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="408ad-110">Выберите веб-сайта или сайтов и на ленте нажмите кнопку **общий доступ**.</span><span class="sxs-lookup"><span data-stu-id="408ad-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="408ad-111">Сайт группы, к которой принадлежит к группе Office 365 или связи сайтов:</span><span class="sxs-lookup"><span data-stu-id="408ad-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="408ad-p103">Эти новые типы сайтов имеют же общего доступа установка в качестве параметра вашей организации, если политика организации не разрешает совместное использование файлов с помощью ссылок, которые не требуют входа в. В этом случае сайты разрешить общий доступ для новых и существующих внешние пользователи, зарегистрированные как. Чтобы изменить параметр для конкретных сайтов, используйте новый центр администрирования SharePoint (Предварительная версия) или PowerShell. [Дополнительные сведения](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="408ad-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="408ad-116">Параметр внешние общего доступа для любого сайта может быть более строгий, чем настроек всей организации, но не больше возможностей, чем параметр всей организации.</span><span class="sxs-lookup"><span data-stu-id="408ad-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

