---
title: Устранение неполадок и ошибок средства миграции SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931131"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="b09a7-102">Устранение неполадок и ошибок средства миграции SharePoint</span><span class="sxs-lookup"><span data-stu-id="b09a7-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="b09a7-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="b09a7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b09a7-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="b09a7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b09a7-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="b09a7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b09a7-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="b09a7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b09a7-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="b09a7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b09a7-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="b09a7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b09a7-109">**Распространенные проблемы и ошибки**</span><span class="sxs-lookup"><span data-stu-id="b09a7-109">**Common issues and errors**</span></span>

<span data-ttu-id="b09a7-110">При использовании средства миграции SharePoint (SPMT) могут возникать некоторые распространенные проблемы и ошибки.</span><span class="sxs-lookup"><span data-stu-id="b09a7-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="b09a7-111">Для получения дополнительных сведений ознакомьтесь со ссылками ниже.</span><span class="sxs-lookup"><span data-stu-id="b09a7-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="b09a7-112">Устранение стандартных проблем и ошибок SMTP</span><span class="sxs-lookup"><span data-stu-id="b09a7-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="b09a7-113">Устранение проблем с установкой SPMT</span><span class="sxs-lookup"><span data-stu-id="b09a7-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)