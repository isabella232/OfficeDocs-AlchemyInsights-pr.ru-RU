---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750677"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="ce165-102">Ограничение доступа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="ce165-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="ce165-103">Существует множество способов ограничения доступа к службам SharePoint Online и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ce165-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="ce165-104">Ниже приведено несколько способов ограничения доступа.</span><span class="sxs-lookup"><span data-stu-id="ce165-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="ce165-105">**Ограничение разрешений**</span><span class="sxs-lookup"><span data-stu-id="ce165-105">**Permission Restriction**</span></span>

<span data-ttu-id="ce165-106">В SharePoint Online и OneDrive для бизнеса мы ограничен доступ к элементам, таким как сайты, файлы и папки, только предоставляя доступ только тем группам и пользователям, у которых есть доступ.</span><span class="sxs-lookup"><span data-stu-id="ce165-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="ce165-107">Настройка разрешений для списка или библиотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="ce165-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="ce165-108">Настройка разрешений сайта в SharePoint</span><span class="sxs-lookup"><span data-stu-id="ce165-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="ce165-109">Изменение разрешений для вложенной папки</span><span class="sxs-lookup"><span data-stu-id="ce165-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="ce165-110">Управление доступом с неуправляемых устройств</span><span class="sxs-lookup"><span data-stu-id="ce165-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="ce165-111">В SharePoint или глобальном администраторе в Office 365 вы можете заблокировать или ограничить доступ к контенту SharePoint и OneDrive с неуправляемых устройств (не с помощью гибридной среды AD или в Intune).</span><span class="sxs-lookup"><span data-stu-id="ce165-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="ce165-112">**Ограничение расположения в сети**</span><span class="sxs-lookup"><span data-stu-id="ce165-112">**Network Location Restriction**</span></span>

<span data-ttu-id="ce165-113">Администратор ИТ-администраторов может управлять доступом к ресурсам SharePoint и OneDrive на основе определенных сетевых расположений, которым вы доверяете.</span><span class="sxs-lookup"><span data-stu-id="ce165-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="ce165-114">Это также называется политикой на основе расположения.</span><span class="sxs-lookup"><span data-stu-id="ce165-114">This is also known as location-based policy.</span></span> <span data-ttu-id="ce165-115">Дополнительные сведения см. в статье [Управление доступом к данным SharePoint Online и OneDrive в зависимости от расположения в сети](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="ce165-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="ce165-116">**Ограничение блокировки сайта**</span><span class="sxs-lookup"><span data-stu-id="ce165-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="ce165-117">В SharePoint Online вы можете заблокировать семейство веб-сайтов, поэтому доступ к нему у него нет.</span><span class="sxs-lookup"><span data-stu-id="ce165-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="ce165-118">Это задается с помощью PowerShell и [командной консоли SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) с помощью свойства [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="ce165-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="ce165-119">**Запретить пользователям создавать сайты или дочерние сайты**</span><span class="sxs-lookup"><span data-stu-id="ce165-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="ce165-120">Администратор SharePoint или глобальный администратор Office 365 позволяют пользователям создавать собственные сайты SharePoint и администрировать их, определять, какие сайты могут создаваться, и указывать расположение сайтов.</span><span class="sxs-lookup"><span data-stu-id="ce165-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="ce165-121">Дополнительные сведения см. в статье [Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="ce165-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

