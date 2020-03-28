---
title: Регулирование во время миграции SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958911"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="ad237-102">Регулирование SharePoint</span><span class="sxs-lookup"><span data-stu-id="ad237-102">SharePoint throttling</span></span>

<span data-ttu-id="ad237-103">**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ad237-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ad237-104">**Регулирование SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="ad237-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="ad237-p101">для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования. Пределы регулирования количество пользовательских действий или одновременных звонков (с скриптах или программах) для предотвращения чрезмерного использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad237-p101">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="ad237-107">Для получения дополнительной информации, пожалуйста, посетите ссылки ниже:</span><span class="sxs-lookup"><span data-stu-id="ad237-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="ad237-108">Как избежать регулирования или блокировки в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ad237-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="ad237-109">Миграция данных и регулирование SPO</span><span class="sxs-lookup"><span data-stu-id="ad237-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="ad237-110">SharePoint Online и скорость миграции в OneDrive</span><span class="sxs-lookup"><span data-stu-id="ad237-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="ad237-111">Реализация регулирования SharePoint Online путем экспоненциального отхода</span><span class="sxs-lookup"><span data-stu-id="ad237-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="ad237-112">Планирование и тестирование загрузки SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ad237-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="ad237-113">Я испытываю низкую производительность или удушение во время миграции</span><span class="sxs-lookup"><span data-stu-id="ad237-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)