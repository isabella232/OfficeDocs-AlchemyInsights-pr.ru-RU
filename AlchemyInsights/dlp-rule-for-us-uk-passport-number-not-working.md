---
title: Правило защиты от потери данных для номера паспорта США и Великобритании не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404394"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="2e7ab-102">Проблемы с номерами паспорта DLP-US/Великобритании</span><span class="sxs-lookup"><span data-stu-id="2e7ab-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="2e7ab-103">Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер паспорта США/Великобритании** при использовании типа конфиденциальной информации DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="2e7ab-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2e7ab-104">Если это так, убедитесь в том, что содержимое содержит необходимые сведения о том, какие параметры политики DLP ищет при оценке.</span><span class="sxs-lookup"><span data-stu-id="2e7ab-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="2e7ab-105">Например, для политики **номера паспорта США и Великобритании** , настроенной на уровне вероятности 75%, оцениваются и должны быть обнаружены для правила, которое необходимо активировать</span><span class="sxs-lookup"><span data-stu-id="2e7ab-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="2e7ab-106">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девять цифр</span><span class="sxs-lookup"><span data-stu-id="2e7ab-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="2e7ab-107">**[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девять последовательных цифр</span><span class="sxs-lookup"><span data-stu-id="2e7ab-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="2e7ab-108">**[КонтрольНая сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Нет, контрольная сумма отсутствует</span><span class="sxs-lookup"><span data-stu-id="2e7ab-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="2e7ab-109">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Политика защиты от потери данных — 75% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:</span><span class="sxs-lookup"><span data-stu-id="2e7ab-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="2e7ab-110">функция Func_usa_uk_passport находит содержимое, которое соответствует шаблону;</span><span class="sxs-lookup"><span data-stu-id="2e7ab-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="2e7ab-111">находится ключевое слово из Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="2e7ab-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="2e7ab-112">Например, следующий пример вызывает срабатывание политики **номеров паспортов для США и Великобритании** : номер паспорта США 123456789</span><span class="sxs-lookup"><span data-stu-id="2e7ab-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="2e7ab-113">Дополнительные сведения о том, что требуется для обнаружения номера паспорта US/Великобритании для вашего контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальНой информации для номера паспорта США и Великобритании](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="2e7ab-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="2e7ab-114">Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальНой информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2e7ab-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

