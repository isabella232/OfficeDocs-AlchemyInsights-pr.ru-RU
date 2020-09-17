---
title: Создание сайта SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806952"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="53121-102">Создание сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="53121-102">Create a SharePoint site</span></span>

<span data-ttu-id="53121-103">Создание сайтов и управление ими из [активных сайтов](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) в центре администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="53121-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="53121-104">Дополнительные сведения см в разделе [Управление сайтами в новом центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="53121-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="53121-105">Использованию</span><span class="sxs-lookup"><span data-stu-id="53121-105">Tips:</span></span>

- <span data-ttu-id="53121-106">**Невозможно** создать сайт с таким же URL-адресом существующего сайта.</span><span class="sxs-lookup"><span data-stu-id="53121-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="53121-107">Если вы удалили сайт и хотите повторно использовать URL-адрес, то удаленный сайт по-прежнему будет существовать в разделе [удаленные сайты](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="53121-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="53121-108">Чтобы повторно использовать URL-адрес, необходимо окончательно удалить сайт.</span><span class="sxs-lookup"><span data-stu-id="53121-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="53121-109">Чтобы полностью удалить сайт с помощью PowerShell, просмотрите пример командлета [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="53121-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="53121-110">Некоторые пользователи могут не иметь возможность создавать сайт.</span><span class="sxs-lookup"><span data-stu-id="53121-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="53121-111">[В разделе Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="53121-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="53121-112">Возможно, сайт зависает при **создании** дольше, чем ожидалось.</span><span class="sxs-lookup"><span data-stu-id="53121-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="53121-113">Если вы пропустили эту ошибку более 24 часов, запишите запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="53121-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="53121-114">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="53121-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="53121-115">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="53121-115">Please give us at least 24 hours to complete a solution.</span></span>
