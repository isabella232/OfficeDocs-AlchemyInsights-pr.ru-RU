---
title: Правила защиты от потери данных для США / номер паспорта (Великобритания) не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786711"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="fa39b-102">Проблемы с DLP - США / номера паспортов (Великобритания)</span><span class="sxs-lookup"><span data-stu-id="fa39b-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="fa39b-p101">Возникают проблемы с **Предотвращения потери данных (DLP)** не работает контента, содержащий **США / номер паспорта (Великобритания)** при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что ваш контент содержит необходимые сведения для что выполняет поиск политики защиты от потери данных при вычислении ее.</span><span class="sxs-lookup"><span data-stu-id="fa39b-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="fa39b-105">Например, для **США / номер паспорта (Великобритания)** политику, настроенную с уровень вероятности 75%, перечисленные ниже вычисляются и необходимо наличие для правила для запуска</span><span class="sxs-lookup"><span data-stu-id="fa39b-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="fa39b-106">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девяти цифр</span><span class="sxs-lookup"><span data-stu-id="fa39b-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="fa39b-107">**[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девять последовательных цифр</span><span class="sxs-lookup"><span data-stu-id="fa39b-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="fa39b-108">**[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Нет, не контрольной суммой</span><span class="sxs-lookup"><span data-stu-id="fa39b-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="fa39b-109">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Политики защиты от потери данных — 75% уверены в том, что этот тип конфиденциальных данных обнаружил if в рамках близости 300 знаков:</span><span class="sxs-lookup"><span data-stu-id="fa39b-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="fa39b-110">функция Func_usa_uk_passport находит содержимое, которое соответствует шаблону;</span><span class="sxs-lookup"><span data-stu-id="fa39b-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="fa39b-111">находится ключевое слово из Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="fa39b-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="fa39b-112">Например, следующий пример приведет к запуску для **США / номер паспорта (Великобритания)** политики: номер паспорта США 123456789</span><span class="sxs-lookup"><span data-stu-id="fa39b-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="fa39b-113">Для получения дополнительных сведений о что является необходимым для США / номер паспорта (Великобритания) для обнаружения для содержимого, в следующем разделе в этой статье: [что конфиденциальные сведения типов внешнего вида для США / номер паспорта (Великобритания)](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="fa39b-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="fa39b-114">С помощью типа различных встроенных конфиденциальной информации, обратитесь к следующей статье сведения на что является необходимым для других типов: [Поиск что конфиденциальные сведения типов](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fa39b-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

