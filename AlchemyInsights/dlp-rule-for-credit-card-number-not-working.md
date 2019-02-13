---
title: Правила защиты от потери данных для номер кредитной карты не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919093"
---
<span data-ttu-id="9189f-p101">Возникают проблемы с **Предотвращения потери данных (DLP)** не работает для контента, содержащий **Номер кредитной карты** , при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что ваш контент содержит необходимые сведения для запуска политики защиты от потери данных при вычислении ее. Например **данные о банковской карте политики** , настроенной с уровень вероятности 85%, следующие вычисляются и необходимо наличие для правила для запуска:</span><span class="sxs-lookup"><span data-stu-id="9189f-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="9189f-105">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, которые могут иметь формат или неформатированные (dddddddddddddddd) и должно пройти проверку Luhn.</span><span class="sxs-lookup"><span data-stu-id="9189f-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="9189f-106">**[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Шаблон очень сложным и надежным, обнаруживает карты из всех основных торговых марок по всему миру, включая Visa, Mastercard, обнаружение карточки, JCB, American Express, подарочные сертификаты и diner карты.</span><span class="sxs-lookup"><span data-stu-id="9189f-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="9189f-107">**[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, контрольная сумма Luhn</span><span class="sxs-lookup"><span data-stu-id="9189f-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="9189f-108">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Политика защиты от потери данных — это 85% уверены в том, что этот тип конфиденциальных данных обнаружил if в рамках близости 300 знаков:</span><span class="sxs-lookup"><span data-stu-id="9189f-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="9189f-109">Функция Func_credit_card находит содержимое, которое соответствует шаблону;</span><span class="sxs-lookup"><span data-stu-id="9189f-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="9189f-110">Верно одно из условий ниже:</span><span class="sxs-lookup"><span data-stu-id="9189f-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="9189f-111">найдено ключевое слово из Keyword_cc_verification;</span><span class="sxs-lookup"><span data-stu-id="9189f-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="9189f-112">Найдено ключевого слова из Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="9189f-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="9189f-113">функция Func_expiration_date находит дату в правильном формате.</span><span class="sxs-lookup"><span data-stu-id="9189f-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="9189f-114">Контрольная сумма передает</span><span class="sxs-lookup"><span data-stu-id="9189f-114">The checksum passes</span></span>
    
    <span data-ttu-id="9189f-115">Например следующий пример приведет к запуску для политики номер кредитной карты защиты от потери данных:</span><span class="sxs-lookup"><span data-stu-id="9189f-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="9189f-116">Visa: 7352 3952 3647 4485</span><span class="sxs-lookup"><span data-stu-id="9189f-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="9189f-117">Действительно до: 2/2009 г.</span><span class="sxs-lookup"><span data-stu-id="9189f-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="9189f-118">Дополнительные сведения о что является необходимым для **Номер кредитной карты** для обнаружения для содержимого в следующем разделе в этой статье: [Что конфиденциальные сведения типов искать данные о банковской карте #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="9189f-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="9189f-119">С помощью типа различных встроенных конфиденциальной информации, обратитесь к следующей статье сведения на что является необходимым для других типов: [Поиск что конфиденциальные сведения типов](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="9189f-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

