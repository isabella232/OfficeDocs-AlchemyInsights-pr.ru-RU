---
title: Удаление сайта SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/24/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c060815d-1d3f-4a13-81c2-0377bbeda202
ms.openlocfilehash: f6ee16a20f2280ba4d8d28ab3fdb4672cd9963b5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927589"
---
# <a name="delete-a-sharepoint-site"></a><span data-ttu-id="cd577-102">Удаление сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="cd577-102">Delete a SharePoint site</span></span>
 <span data-ttu-id="cd577-103">**Удаление сайтов в центре администрирования SharePoint**</span><span class="sxs-lookup"><span data-stu-id="cd577-103">**Delete sites from the new SharePoint admin center**</span></span>
  
<span data-ttu-id="cd577-p101">Удаление активного сайта, перейдите в текущем Центр администрирования SharePoint, нажмите кнопку «Попробуйте прямо сейчас» в правом верхнем углу. Выберите **сайты Active**, выберите сайт и выберите команду **Удалить**. [Просмотр и восстановления удаленных сайтов в центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)выберите **удаленных сайтов**. Дополнительные сведения в разделе [Управление узлами в центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span><span class="sxs-lookup"><span data-stu-id="cd577-p101">To delete an active site, go to the current SharePoint admin center, click "Try it now" in the upper right. Select **Active sites**, select the site, and then select **Delete**. To [view and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center), select **Deleted sites**. For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span></span>
  
<span data-ttu-id="cd577-p102">**Важные:** Если узел является частью политику хранения, не можно удалить ее, пока сайт не будет удалено из [безопасности &amp; Центр администрирования соответствия](https://protection.office.com/?rfr=AdminCenter#/homepage). Дополнительные сведения в разделе [Обзор политик хранения](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) .</span><span class="sxs-lookup"><span data-stu-id="cd577-p102">**Important:** If the site is part of a retention policy, you may not be able to delete it until the site is removed from the [Security &amp; Compliance Admin Center](https://protection.office.com/?rfr=AdminCenter#/homepage). See [Overview of Retention Policies](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) for more info.</span></span> 
  
<span data-ttu-id="cd577-110">Советы по:</span><span class="sxs-lookup"><span data-stu-id="cd577-110">Tips:</span></span>
- <span data-ttu-id="cd577-p103">Глобальные "Администраторы" и "Администраторы SharePoint" теперь удаление веб-сайтов, относящихся к **Office 365 группы**. Это приведет к удалению группы и всех его ресурсов, включая почтовый ящик Outlook и календарь и все каналы группами. Дополнительные сведения см.в [Удаление сайта SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="cd577-p103">Global admins and SharePoint admins can now delete sites that belong to an **Office 365 Group**. This will delete the group and all its resources, including the Outlook mailbox and calendar, and any Teams channels. For more info, see [Delete a SharePoint site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span></span>
- <span data-ttu-id="cd577-p104">Для восстановления удаленных сайтов для 93 дней. Обратите внимание на то, что в течение 30 дней, необходимо восстанавливать удаленные группы. Дополнительные сведения см в [представление и восстановления удаленных сайтов](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).</span><span class="sxs-lookup"><span data-stu-id="cd577-p104">You can recover deleted sites for 93 days. Note that deleted groups must be restored within 30 days. For more info, see [View and restore deleted sites](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).</span></span>
- <span data-ttu-id="cd577-117">Чтобы полностью удалить сайт с помощью Powershell, см в примере командлет [Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="cd577-117">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) cmdlet example.</span></span> 
  

