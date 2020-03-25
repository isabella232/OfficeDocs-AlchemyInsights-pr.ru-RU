---
title: Правило DLP для номера кредитной карты не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932456"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d3051-102">Проблемы с DLP с номерами кредитных карт</span><span class="sxs-lookup"><span data-stu-id="d3051-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d3051-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="d3051-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d3051-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="d3051-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d3051-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="d3051-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d3051-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="d3051-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d3051-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="d3051-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d3051-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="d3051-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d3051-109">**Проблемы с DLP с номерами кредитных карт**</span><span class="sxs-lookup"><span data-stu-id="d3051-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d3051-110">Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер кредитной карты** , при использовании типа конфиденциальной информации DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="d3051-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d3051-111">Если это так, убедитесь, что содержимое содержит необходимые сведения, чтобы активировать политику DLP при его оценке.</span><span class="sxs-lookup"><span data-stu-id="d3051-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d3051-112">Например, для **политики кредитных карт** , настроенной с уровнем вероятности 85%, оцениваются и должны быть обнаружены правила для активации правила:</span><span class="sxs-lookup"><span data-stu-id="d3051-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d3051-113">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, которые могут быть форматированными или неформатированными (цццццццццццццццц) и должны пройти проверку Луна.</span><span class="sxs-lookup"><span data-stu-id="d3051-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d3051-114">**[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Очень сложный и надежный шаблон, который находит карты со всех основных торговых марок, включая Visa, MasterCard, обнаружение карт, JCB, американский Express, подарочные сертификаты и карточки Динер.</span><span class="sxs-lookup"><span data-stu-id="d3051-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d3051-115">**[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, контрольная сумма Луна</span><span class="sxs-lookup"><span data-stu-id="d3051-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d3051-116">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Политика защиты от потери данных — 85% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:</span><span class="sxs-lookup"><span data-stu-id="d3051-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d3051-117">Функция Func_credit_card находит содержимое, которое соответствует шаблону;</span><span class="sxs-lookup"><span data-stu-id="d3051-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d3051-118">Верно одно из условий ниже:</span><span class="sxs-lookup"><span data-stu-id="d3051-118">One of the following is true:</span></span>

  - <span data-ttu-id="d3051-119">найдено ключевое слово из Keyword_cc_verification;</span><span class="sxs-lookup"><span data-stu-id="d3051-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d3051-120">Найдено ключевое слово из Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="d3051-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d3051-121">функция Func_expiration_date находит дату в правильном формате.</span><span class="sxs-lookup"><span data-stu-id="d3051-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d3051-122">Контрольная сумма проходит</span><span class="sxs-lookup"><span data-stu-id="d3051-122">The checksum passes</span></span>

    <span data-ttu-id="d3051-123">Например, в приведенном ниже примере запускается политика номеров кредитных карт DLP.</span><span class="sxs-lookup"><span data-stu-id="d3051-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d3051-124">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d3051-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d3051-125">Срок действия: 2/2009</span><span class="sxs-lookup"><span data-stu-id="d3051-125">Expires: 2/2009</span></span>

<span data-ttu-id="d3051-126">Дополнительные сведения о том, что требуется для обнаружения **номера кредитной карты** для контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для карты No](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="d3051-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="d3051-127">Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d3051-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  