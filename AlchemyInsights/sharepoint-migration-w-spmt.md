---
title: Миграция SharePoint с помощью SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931563"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="62185-102">Миграция SharePoint с помощью SPMT</span><span class="sxs-lookup"><span data-stu-id="62185-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="62185-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="62185-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="62185-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="62185-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="62185-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="62185-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="62185-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="62185-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="62185-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="62185-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="62185-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="62185-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="62185-109">**Средство миграции SharePoint**</span><span class="sxs-lookup"><span data-stu-id="62185-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="62185-110">Предназначено для использования при миграции из наименьшего набора файлов в крупномасштабную миграцию в масштабах предприятия, средство миграции SharePoint позволит вам перенести данные в облако и воспользоваться преимуществами новейших функций совместной работы, анализа и решения для обеспечения безопасности с помощью Office 365.</span><span class="sxs-lookup"><span data-stu-id="62185-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="62185-111">Скачивание и установка средства миграции SharePoint</span><span class="sxs-lookup"><span data-stu-id="62185-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="62185-112">Устранение стандартных проблем и ошибок SMTP</span><span class="sxs-lookup"><span data-stu-id="62185-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="62185-113">Устранение неполадок с установкой SPMT</span><span class="sxs-lookup"><span data-stu-id="62185-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
