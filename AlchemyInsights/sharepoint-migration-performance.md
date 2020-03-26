---
title: Производительность миграции SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932247"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="5dd6e-102">Производительность миграции SharePoint</span><span class="sxs-lookup"><span data-stu-id="5dd6e-102">SharePoint migration performance</span></span>

<span data-ttu-id="5dd6e-103">**Важно!** Многие клиенты SharePoint Online и OneDrive с помощью службы запускают критически важные для бизнеса приложения, которые выполняются в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5dd6e-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5dd6e-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5dd6e-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5dd6e-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5dd6e-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5dd6e-109">**Производительность миграции**</span><span class="sxs-lookup"><span data-stu-id="5dd6e-109">**Migration performance**</span></span>

<span data-ttu-id="5dd6e-p103">На производительность миграции может влиять сетевая инфраструктура, размер файла, время миграции и регулирование. Понимание этого поможет вам планировать миграцию и сделать ее максимально эффективной.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="5dd6e-112">Дополнительные сведения см. по ссылкам ниже.</span><span class="sxs-lookup"><span data-stu-id="5dd6e-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="5dd6e-113">SharePoint Online и скорость миграции в ODB</span><span class="sxs-lookup"><span data-stu-id="5dd6e-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="5dd6e-114">Как избежать регулирования или блокировки в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5dd6e-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="5dd6e-115">Скачивание и установка средства миграции SharePoint</span><span class="sxs-lookup"><span data-stu-id="5dd6e-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
