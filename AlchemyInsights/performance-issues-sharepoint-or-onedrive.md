---
title: Проблемы с производительностью — SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068428"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a541f-102">Медленный, недоступный или недоступный для нескольких пользователей SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="a541f-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="a541f-103">SharePoint или OneDrive может быть медленной, недоступен или недоступен или может отображать недоступные службы или 503 ошибок, по нескольким причинам:</span><span class="sxs-lookup"><span data-stu-id="a541f-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="a541f-104">Если сайт SharePoint или OneDrive работает медленнее или задержано для нескольких пользователей, может возникнуть временная ошибка службы, из-за которой при доступе пользователей к сайтам SharePoint или контенту в OneDrive возникают временные задержки или ошибки навигации.</span><span class="sxs-lookup"><span data-stu-id="a541f-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="a541f-105">Просмотрите [панель мониторинга работоспособности службы](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить, влияет ли ваша организация на работу.</span><span class="sxs-lookup"><span data-stu-id="a541f-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="a541f-106">При попытке перейти к сайтам SharePoint или OneDrive пользователи могут получить сообщение о *занятости сервера 503* .</span><span class="sxs-lookup"><span data-stu-id="a541f-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="a541f-107">Эта ошибка может быть вызвана регулированием в службе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a541f-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a541f-108">для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования.</span><span class="sxs-lookup"><span data-stu-id="a541f-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a541f-109">Пределы регулирования количество пользовательских действий или одновременных звонков (с скриптах или программах) для предотвращения чрезмерного использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a541f-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="a541f-110">Для получения дополнительных сведений об регулированиях см. [Избегайте регулирования или блокировки в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="a541f-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="a541f-111">При низкой производительности с помощью **классического** или **современного** сайта или страницы SharePoint используйте [средство диагностики страниц](https://aka.ms/perftool) для анализа страниц.</span><span class="sxs-lookup"><span data-stu-id="a541f-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="a541f-112">Если вы по-прежнему работает с низкой производительностью, ознакомьтесь с ресурсами в нижней части этой статьи: " [Введение в настройку производительности для SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334) ".</span><span class="sxs-lookup"><span data-stu-id="a541f-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  