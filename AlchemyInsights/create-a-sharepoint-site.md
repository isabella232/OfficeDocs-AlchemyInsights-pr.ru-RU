---
title: Создание сайта SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769604"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="e92a3-102">Создание сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="e92a3-102">Create a SharePoint site</span></span>

<span data-ttu-id="e92a3-103">Сведения о создании сайтов SharePoint можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="e92a3-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="e92a3-104">[Управление сайтами в новом центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): сведения о возможностях создания сайтов, в том числе о создании классического сайта или сайта Teams, не включающего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="e92a3-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="e92a3-105">[Создайте сайт группы в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Узнайте, как создать сайт группы.</span><span class="sxs-lookup"><span data-stu-id="e92a3-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="e92a3-106">[Создание информационного сайта в SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Узнайте, как создать сайт для общения.</span><span class="sxs-lookup"><span data-stu-id="e92a3-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="e92a3-107">[Управление сайтами в новом центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Узнайте, как создать классический сайт или сайт группы, который не включает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="e92a3-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="e92a3-108">**Использованию**</span><span class="sxs-lookup"><span data-stu-id="e92a3-108">**Tips:**</span></span>
- <span data-ttu-id="e92a3-109">Невозможно создать сайт с таким же URL-адресом существующего сайта.</span><span class="sxs-lookup"><span data-stu-id="e92a3-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="e92a3-110">Если вы удалили сайт и хотите повторно использовать URL-адрес, то удаленный сайт по-прежнему будет существовать в разделе **удаленные сайты**.</span><span class="sxs-lookup"><span data-stu-id="e92a3-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="e92a3-111">Чтобы управлять удаленными сайтами, [удалите сайт](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="e92a3-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="e92a3-112">Чтобы полностью удалить сайт с помощью PowerShell, просмотрите пример командлета [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="e92a3-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="e92a3-113">Некоторые пользователи могут не иметь возможность создавать сайт.</span><span class="sxs-lookup"><span data-stu-id="e92a3-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="e92a3-114">[В разделе Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="e92a3-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="e92a3-115">Возможно, сайт зависает при **создании** дольше, чем ожидалось.</span><span class="sxs-lookup"><span data-stu-id="e92a3-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="e92a3-116">Если вы пропустили эту ошибку более 24 часов, запишите запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="e92a3-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e92a3-117">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="e92a3-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e92a3-118">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="e92a3-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="e92a3-119">Если необходимо создать новый сайт группы, который не включает группу Office 365,</span><span class="sxs-lookup"><span data-stu-id="e92a3-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


