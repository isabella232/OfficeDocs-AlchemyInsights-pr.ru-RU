---
title: Современный сайт в качестве корневого сайта
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057763"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="2182a-102">Современный сайт в качестве корневого сайта</span><span class="sxs-lookup"><span data-stu-id="2182a-102">Modern site as root site</span></span>

<span data-ttu-id="2182a-103">Клиенты [целевого выпуска](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) теперь могут активировать интерфейс современного сайта для общения на классическом корневом сайте клиента SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2182a-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="2182a-104">Эту функцию можно активировать, выполнив простой командлет PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2182a-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="2182a-105">При успешном выполнении команд PowerShell корневой сайт будет содержать новую домашнюю страницу сайта для общения.</span><span class="sxs-lookup"><span data-stu-id="2182a-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="2182a-106">Сведения о командлетах и требованиях к функциям PowerShell доступны в статье [Enable – спокоммсите](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="2182a-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="2182a-107">Мы будем постепенно отвлекаться по умолчанию, а не по умолчанию для клиентов, нацеленных на выпуск ранних версий 2019, а развертывание будет доступно в конце июня 2019.</span><span class="sxs-lookup"><span data-stu-id="2182a-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="2182a-108">Продолжайте ссылаться на [Центр сообщений](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) о других новых возможностях с современным интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="2182a-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="2182a-109">**Важно!** не удаляйте классический корневой сайт для создания современного информационного сайта.</span><span class="sxs-lookup"><span data-stu-id="2182a-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="2182a-110">Корпорация Майкрософт не поддерживает этот параметр.</span><span class="sxs-lookup"><span data-stu-id="2182a-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="2182a-111">Удаление корневого сайта сделает все сайты SharePoint в Организации недоступными для всех пользователей, пока не восстановите сайт или не создаст новый сайт с тем же URL-АДРЕСом.</span><span class="sxs-lookup"><span data-stu-id="2182a-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 