---
title: Добавление группы на сайт SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750533"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="314b1-102">Проблемы при создании или группировании подключенных сайтов в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="314b1-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="314b1-103">При создании или повторном создании подключенного к группе сайта возникла пара распространенных проблем.</span><span class="sxs-lookup"><span data-stu-id="314b1-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="314b1-104">Если вы удалили группу и подключенный сайт и хотите создать другой сайт с тем же URL-адресом, необходимо удалить предыдущий сайт без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="314b1-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="314b1-105">Загрузка [командной консоли SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="314b1-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="314b1-106">Более подробную информацию о начале работы с PowerShell можно узнать в статье [Начало работы с помощью командной консоли SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="314b1-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="314b1-107">Удалите сайт из удаленных сайтов с помощью командлета PowerShell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="314b1-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="314b1-108">Если вы создаете сайт, подключенный к группе, и получаете предупреждение о том, что уже существует еще одна группа с таким же псевдонимом, проверьте существующие группы из [центра администрирования Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="314b1-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="314b1-109">Чтобы устранить эту проблему, удалите существующую группу, если она больше не нужна, или создайте сайт с другим назначенным псевдонимом.</span><span class="sxs-lookup"><span data-stu-id="314b1-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="314b1-110">Существуют различные способы создания и использования современных групп с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="314b1-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="314b1-111">Вы можете подключить существующие сайты к группе Office 365.</span><span class="sxs-lookup"><span data-stu-id="314b1-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="314b1-112">Для получения дополнительных сведений обратитесь [к разделу Подключение группы Office 365 с помощью пользователя SharePoint инетерфаце](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="314b1-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="314b1-113">Чтобы создать сайт, подключенный к группе Office 365, необходимо создать сайт группы.</span><span class="sxs-lookup"><span data-stu-id="314b1-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="314b1-114">Более подробную информацию можно узнать [в статье Создание сайта группы в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="314b1-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

