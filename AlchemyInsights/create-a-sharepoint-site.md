---
title: Создание сайта SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: a4c6029c632178136396a91ba9754752dc8f7180
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32407627"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="100e8-102">Создание сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="100e8-102">Create a SharePoint site</span></span>

<span data-ttu-id="100e8-103">Параметры создания сайтов перечислены [в разделе Управление сайтами в новом центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation ) .</span><span class="sxs-lookup"><span data-stu-id="100e8-103">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options.</span></span> <span data-ttu-id="100e8-104">Выберите, чтобы создать [сайт группы](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (который будет создавать группу Office 365) или сайт для [общения](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb).</span><span class="sxs-lookup"><span data-stu-id="100e8-104">Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb).</span></span> <span data-ttu-id="100e8-105">Для создания [классического сайта](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)или нового сайта группы, не включающего группу Office 365, щелкните **другие параметры**.</span><span class="sxs-lookup"><span data-stu-id="100e8-105">To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span> 
  
<span data-ttu-id="100e8-106">Использованию</span><span class="sxs-lookup"><span data-stu-id="100e8-106">Tips:</span></span>
- <span data-ttu-id="100e8-107">*Невозможно создать сайт с таким же URL-АДРЕСом существующего сайта. Если вы удалили сайт и хотите повторно использовать URL-адрес, то удаленный сайт по-прежнему будет существовать в разделе **удаленные сайты**. Чтобы управлять удаленными сайтами, [удалите сайт](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). Чтобы полностью удалить сайт с помощью PowerShell, просмотрите пример командлета [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .*</span><span class="sxs-lookup"><span data-stu-id="100e8-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="100e8-108">*Некоторые пользователи могут не иметь возможность создавать сайт. [В разделе Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span><span class="sxs-lookup"><span data-stu-id="100e8-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="100e8-109">*Возможно, сайт зависает при **создании** дольше, чем ожидалось. Если вы пропустили эту ошибку более 24 часов, запишите запрос в службу поддержки. Во многих случаях мы уже работаем над решением. Отправьте нам по крайней мере 24 часа для завершения решения.*</span><span class="sxs-lookup"><span data-stu-id="100e8-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
