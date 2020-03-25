---
title: Советы политики защиты от потери данных не работают
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932599"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="f33e5-102">Проблемы с подсказкой политики DLP</span><span class="sxs-lookup"><span data-stu-id="f33e5-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="f33e5-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="f33e5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f33e5-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="f33e5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f33e5-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="f33e5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f33e5-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="f33e5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f33e5-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="f33e5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f33e5-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="f33e5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f33e5-109">**Советы по политике защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="f33e5-109">**DLP policy tips**</span></span>

<span data-ttu-id="f33e5-110">При использовании **политик защиты от потери**данных пользователи могут получать уведомления о нарушении политики с помощью **подсказок политики**.</span><span class="sxs-lookup"><span data-stu-id="f33e5-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="f33e5-111">Администраторы могут настроить подсказки политики для отображения при тестировании политики защиты от потери данных или когда политика находится в режиме полной принудительной защиты.</span><span class="sxs-lookup"><span data-stu-id="f33e5-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="f33e5-112">Чтобы настроить подсказки политики для политики защиты от потери данных в центре безопасности и соответствия требованиям в режиме полного применения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="f33e5-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="f33e5-113">Убедитесь, что подсказка политики **включена** для правила DLP, выполнив действия, описанные в [этой статье](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="f33e5-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="f33e5-114">Убедитесь, что **контент соответствует** тому, что **требуется** для запуска правила, описанного в этой [статье.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f33e5-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="f33e5-115">Подсказка политики отображается как в OWA, так и в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f33e5-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="f33e5-116">Однако при использовании **Outlook 2013 или более поздней версии**подсказки политики отображаются только при определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="f33e5-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="f33e5-117">Эти условия перечислены ниже: [Поддерживаемые условия для Outlook 2013 или более поздней версии для отображения подсказок политики](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="f33e5-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="f33e5-118">Дополнительные сведения о подсказках политики DLP: [show policy подсказки для политик защиты от потери](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) данных</span><span class="sxs-lookup"><span data-stu-id="f33e5-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  