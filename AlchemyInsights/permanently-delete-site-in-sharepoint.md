---
title: Навсегда удалить сайт в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955240"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="d1dec-102">Навсегда удалить сайт в SharePoint</span><span class="sxs-lookup"><span data-stu-id="d1dec-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="d1dec-103">Чтобы повторно использовать URL-адрес на удаленном сайте (чтобы повторно создать сайт) или окончательно удалить сайт, так как он больше не используется, можно использовать **окончательно удалить** из нового центра администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1dec-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="d1dec-104">Перейдите на страницу [Удаленные сайты нового центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) и войдите в систему, используя учетную запись с правами администратора вашей организации.</span><span class="sxs-lookup"><span data-stu-id="d1dec-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="d1dec-105">В левом столбце выберите сайт.</span><span class="sxs-lookup"><span data-stu-id="d1dec-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="d1dec-106">Нажмите кнопку **окончательно удалить**.</span><span class="sxs-lookup"><span data-stu-id="d1dec-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="d1dec-107">**Примечание**: сайты, подключенные к группе, нельзя удалить из Центра администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1dec-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="d1dec-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) необходимо будет использовать вместо этого.</span><span class="sxs-lookup"><span data-stu-id="d1dec-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="d1dec-109">Для получения дополнительной информации см. [Окончательно удалить сайт](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="d1dec-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
