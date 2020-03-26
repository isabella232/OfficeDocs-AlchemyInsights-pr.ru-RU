---
title: Общие рекомендации по производительности миграции
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932491"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="8eedc-102">Общие рекомендации по производительности миграции</span><span class="sxs-lookup"><span data-stu-id="8eedc-102">General migration performance guidance</span></span>

<span data-ttu-id="8eedc-103">**Важно!** Многие клиенты SharePoint Online и OneDrive с помощью службы запускают критически важные для бизнеса приложения, которые выполняются в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="8eedc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8eedc-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="8eedc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8eedc-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="8eedc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8eedc-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="8eedc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8eedc-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="8eedc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8eedc-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="8eedc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8eedc-109">**Рекомендации по производительности миграции**</span><span class="sxs-lookup"><span data-stu-id="8eedc-109">**Migration performance guidance**</span></span>

<span data-ttu-id="8eedc-p103">На производительность миграции может влиять сетевая инфраструктура, размер файла, время миграции и регулирование. Понимание этого поможет вам планировать миграцию и сделать ее максимально эффективной.</span><span class="sxs-lookup"><span data-stu-id="8eedc-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="8eedc-112">Общие рекомендации по производительности миграции</span><span class="sxs-lookup"><span data-stu-id="8eedc-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
