---
title: Дополнительные сведения о проблемах защиты от потери данных
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932707"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="787f3-102">Сведения о проблемах с DLP</span><span class="sxs-lookup"><span data-stu-id="787f3-102">Information about DLP issues</span></span>

<span data-ttu-id="787f3-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="787f3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="787f3-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="787f3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="787f3-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="787f3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="787f3-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="787f3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="787f3-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="787f3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="787f3-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="787f3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="787f3-109">**Сведения о политике защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="787f3-109">**Information on DLP policy**</span></span>

<span data-ttu-id="787f3-110">С помощью политики защиты от потери данных можно определять, отслеживать и автоматически защищать конфиденциальные данные в Office 365.</span><span class="sxs-lookup"><span data-stu-id="787f3-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="787f3-111">Для получения дополнительных сведений посетите следующие ссылки:</span><span class="sxs-lookup"><span data-stu-id="787f3-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="787f3-112">Общие сведения о защите от потери данных</span><span class="sxs-lookup"><span data-stu-id="787f3-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="787f3-113">Что позволяют искать типы конфиденциальной информации</span><span class="sxs-lookup"><span data-stu-id="787f3-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="787f3-114">Создание специальных типов конфиденциальных данных</span><span class="sxs-lookup"><span data-stu-id="787f3-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="787f3-115">Отправка уведомлений по электронной почте и отображение подсказок политики</span><span class="sxs-lookup"><span data-stu-id="787f3-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="787f3-116">Защита файлов SharePoint Online с помощью меток хранения и DLP</span><span class="sxs-lookup"><span data-stu-id="787f3-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="787f3-117">DLP и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="787f3-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="787f3-118">Чтобы протестировать данные со встроенным или настраиваемым типом конфиденциальной информации, используйте параметр **тип теста** в разделе **классификация** > **типов конфиденциальной**информации.</span><span class="sxs-lookup"><span data-stu-id="787f3-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="787f3-119">Дополнительные [сведения см.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="787f3-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>