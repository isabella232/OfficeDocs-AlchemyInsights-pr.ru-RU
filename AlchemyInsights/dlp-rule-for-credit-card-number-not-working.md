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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977211"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="f2473-102">Проблемы с DLP с номерами кредитных карт</span><span class="sxs-lookup"><span data-stu-id="f2473-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="f2473-103">**Важно!** в это незначительное время мы предоставим вам рекомендации по включению служб SharePoint Online и OneDrive, чтобы получить дополнительные сведения о [временных функциях SharePoint](https://aka.ms/ODSPAdjustments) Online.</span><span class="sxs-lookup"><span data-stu-id="f2473-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f2473-104">**Проблемы с DLP с номерами кредитных карт**</span><span class="sxs-lookup"><span data-stu-id="f2473-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="f2473-105">Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер кредитной карты** , при использовании типа конфиденциальной информации DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="f2473-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f2473-106">Если это так, убедитесь, что содержимое содержит необходимые сведения, чтобы активировать политику DLP при его оценке.</span><span class="sxs-lookup"><span data-stu-id="f2473-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="f2473-107">Например, для **политики кредитных карт** , настроенной с уровнем вероятности 85%, оцениваются и должны быть обнаружены правила для активации правила:</span><span class="sxs-lookup"><span data-stu-id="f2473-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f2473-108">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, которые могут быть форматированными или неформатированными (цццццццццццццццц) и должны пройти проверку Луна.</span><span class="sxs-lookup"><span data-stu-id="f2473-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="f2473-109">**[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Очень сложный и надежный шаблон, который находит карты со всех основных торговых марок, включая Visa, MasterCard, обнаружение карт, JCB, американский Express, подарочные сертификаты и карточки Динер.</span><span class="sxs-lookup"><span data-stu-id="f2473-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="f2473-110">**[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, контрольная сумма Луна</span><span class="sxs-lookup"><span data-stu-id="f2473-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="f2473-111">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Политика защиты от потери данных — 85% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:</span><span class="sxs-lookup"><span data-stu-id="f2473-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f2473-112">Функция Func_credit_card находит содержимое, которое соответствует шаблону;</span><span class="sxs-lookup"><span data-stu-id="f2473-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f2473-113">Верно одно из условий ниже:</span><span class="sxs-lookup"><span data-stu-id="f2473-113">One of the following is true:</span></span>

  - <span data-ttu-id="f2473-114">найдено ключевое слово из Keyword_cc_verification;</span><span class="sxs-lookup"><span data-stu-id="f2473-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="f2473-115">Найдено ключевое слово из Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="f2473-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="f2473-116">функция Func_expiration_date находит дату в правильном формате.</span><span class="sxs-lookup"><span data-stu-id="f2473-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="f2473-117">Контрольная сумма проходит</span><span class="sxs-lookup"><span data-stu-id="f2473-117">The checksum passes</span></span>

    <span data-ttu-id="f2473-118">Например, в приведенном ниже примере запускается политика номеров кредитных карт DLP.</span><span class="sxs-lookup"><span data-stu-id="f2473-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="f2473-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="f2473-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="f2473-120">Срок действия: 2/2009</span><span class="sxs-lookup"><span data-stu-id="f2473-120">Expires: 2/2009</span></span>

<span data-ttu-id="f2473-121">Дополнительные сведения о том, что требуется для обнаружения **номера кредитной карты** для контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для карты No](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="f2473-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="f2473-122">Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f2473-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  