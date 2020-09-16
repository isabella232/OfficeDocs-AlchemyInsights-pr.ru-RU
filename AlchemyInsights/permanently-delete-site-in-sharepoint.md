---
title: Навсегда удалить сайт в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771734"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="e4cf4-102">Навсегда удалить сайт в SharePoint</span><span class="sxs-lookup"><span data-stu-id="e4cf4-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="e4cf4-103">Чтобы повторно использовать URL-адрес на удаленном сайте (чтобы повторно создать сайт) или окончательно удалить сайт, так как он больше не используется, можно использовать **окончательно удалить** из нового центра администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e4cf4-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="e4cf4-104">Перейдите на страницу [Удаленные сайты нового центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) и войдите в систему, используя учетную запись с правами администратора вашей организации.</span><span class="sxs-lookup"><span data-stu-id="e4cf4-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="e4cf4-105">В левом столбце выберите сайт.</span><span class="sxs-lookup"><span data-stu-id="e4cf4-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="e4cf4-106">Нажмите кнопку **окончательно удалить**.</span><span class="sxs-lookup"><span data-stu-id="e4cf4-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="e4cf4-107">**Примечание**: сайты, подключенные к группе, нельзя удалить из Центра администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e4cf4-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="e4cf4-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) необходимо будет использовать вместо этого.</span><span class="sxs-lookup"><span data-stu-id="e4cf4-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="e4cf4-109">Для получения дополнительной информации см. [Окончательно удалить сайт](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="e4cf4-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
