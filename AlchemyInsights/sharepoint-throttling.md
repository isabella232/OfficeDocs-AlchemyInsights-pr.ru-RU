---
title: Регулирование SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931455"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5725e-102">Регулирование SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5725e-102">SharePoint Online throttling</span></span>

<span data-ttu-id="5725e-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="5725e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5725e-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="5725e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5725e-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="5725e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5725e-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="5725e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5725e-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="5725e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5725e-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="5725e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5725e-109">**Регулирование SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="5725e-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="5725e-110">для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования.</span><span class="sxs-lookup"><span data-stu-id="5725e-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5725e-111">Пределы регулирования количество пользовательских действий или одновременных звонков (с скриптах или программах) для предотвращения чрезмерного использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5725e-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5725e-112">Для получения дополнительных сведений перейдите по приведенным ниже ссылкам.</span><span class="sxs-lookup"><span data-stu-id="5725e-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="5725e-113">Как избежать регулирования или блокировки в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5725e-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="5725e-114">Миграция данных и SPO регулирование</span><span class="sxs-lookup"><span data-stu-id="5725e-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="5725e-115">SharePoint Online и скорость миграции в OneDrive</span><span class="sxs-lookup"><span data-stu-id="5725e-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="5725e-116">Реализация регулирования SharePoint Online путем экспоненциального отхода</span><span class="sxs-lookup"><span data-stu-id="5725e-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="5725e-117">Планирование и тестирование загрузки SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5725e-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

