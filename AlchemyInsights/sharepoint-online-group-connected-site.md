---
title: Добавление группы на сайт SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770364"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="295e7-102">Проблемы при создании сайта с подключением к группе в SharePoint</span><span class="sxs-lookup"><span data-stu-id="295e7-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="295e7-103">Некоторые распространенные проблемы, возникающие при создании или повторном создании подключенного к группе сайта.</span><span class="sxs-lookup"><span data-stu-id="295e7-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="295e7-104">Если вы удалили группу и подключенный сайт и хотите создать другой сайт с тем же URL-адресом, необходимо удалить предыдущий сайт без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="295e7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="295e7-105">Загрузка [командной консоли SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="295e7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="295e7-106">Более подробную информацию о начале работы с PowerShell можно узнать в статье [Начало работы с консолью управления SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="295e7-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="295e7-107">Удалите сайт из удаленных сайтов с помощью командлета PowerShell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="295e7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="295e7-108">Для окончательного удаления групп сайтов требуется PowerShell.</span><span class="sxs-lookup"><span data-stu-id="295e7-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="295e7-109">Если вы создаете сайт, подключенный к группе, и получаете предупреждение: **уже существует другая группа с таким же псевдонимом**, проверьте существующие группы из [центра администрирования Office 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="295e7-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="295e7-110">Чтобы устранить эту проблему, удалите существующую группу, если она больше не нужна, или создайте сайт с другим назначенным псевдонимом.</span><span class="sxs-lookup"><span data-stu-id="295e7-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="295e7-111">Существуют различные способы создания и использования современных групп с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="295e7-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="295e7-112">Вы можете подключить существующие сайты к группе Office 365.</span><span class="sxs-lookup"><span data-stu-id="295e7-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="295e7-113">Для получения дополнительных сведений обратитесь [к разделу Подключение группы Office 365 с помощью пользовательского интерфейса SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="295e7-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="295e7-114">Чтобы создать сайт, подключенный к группе Office 365, необходимо создать [сайт группы](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="295e7-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
