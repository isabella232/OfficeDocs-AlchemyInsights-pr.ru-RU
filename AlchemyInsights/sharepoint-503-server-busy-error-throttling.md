---
title: Регулирование SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931239"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="493c1-102">Регулирование SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="493c1-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="493c1-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="493c1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="493c1-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="493c1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="493c1-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="493c1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="493c1-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="493c1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="493c1-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="493c1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="493c1-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="493c1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="493c1-109">**503 Сервер занят**</span><span class="sxs-lookup"><span data-stu-id="493c1-109">**503 server is busy error**</span></span>

<span data-ttu-id="493c1-110">При попытке перейти к сайтам SharePoint или OneDrive пользователи могут получить сообщение о занятости сервера 503.</span><span class="sxs-lookup"><span data-stu-id="493c1-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="493c1-111">Эта ошибка может быть вызвана регулированием в службе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="493c1-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="493c1-112">для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования.</span><span class="sxs-lookup"><span data-stu-id="493c1-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="493c1-113">Пределы регулирования количество пользовательских действий или одновременных звонков (с скриптах или программах) для предотвращения чрезмерного использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="493c1-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="493c1-114">Для получения дополнительных сведений об регулированиях см. [Избегайте регулирования или блокировки в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="493c1-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="493c1-115">Если вы считаете, что эта ошибка не связана с регулированием, вы можете проверить, есть ли активное обслуживание клиента, перейдя в [Центр сообщений](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="493c1-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="493c1-116">Наконец, убедитесь, что вы посещаете страницу [работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth) , чтобы проверить, какие рекомендации и происшествия могут возникать.</span><span class="sxs-lookup"><span data-stu-id="493c1-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

