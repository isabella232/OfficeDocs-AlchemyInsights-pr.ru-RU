---
title: Перенос параметров в SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932743"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="9e210-102">Перенос параметров в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9e210-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="9e210-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="9e210-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9e210-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="9e210-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9e210-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="9e210-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9e210-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="9e210-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9e210-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="9e210-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9e210-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="9e210-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9e210-109">**Варианты миграции**</span><span class="sxs-lookup"><span data-stu-id="9e210-109">**Migration options**</span></span>

<span data-ttu-id="9e210-110">Существуют различные параметры для переноса контента в SharePoint Online, в зависимости от размера и количества файлов, которые необходимо переместить, просмотрите список параметров, [расположенных здесь](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="9e210-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="9e210-111">Для получения дополнительных сведений о переносе контента перейдите по приведенным ниже ссылкам.</span><span class="sxs-lookup"><span data-stu-id="9e210-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="9e210-112">Средство миграции SharePoint</span><span class="sxs-lookup"><span data-stu-id="9e210-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="9e210-113">Начало работы с диспетчером переноса данных</span><span class="sxs-lookup"><span data-stu-id="9e210-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="9e210-114">Скорость миграции SharePoint Online и ODB</span><span class="sxs-lookup"><span data-stu-id="9e210-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="9e210-115">Как избежать регулирования или блокировки в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9e210-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="9e210-116">Средство оценки миграции SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="9e210-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="9e210-117">**Note**: в настоящее время средство миграции SharePoint поддерживает только миграцию с SharePoint 2010 и 2013.</span><span class="sxs-lookup"><span data-stu-id="9e210-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="9e210-118">В настоящее время не поддерживаются версии 2016 или 2019.</span><span class="sxs-lookup"><span data-stu-id="9e210-118">Version 2016 or 2019 are not supported at this time.</span></span>
