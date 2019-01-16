---
title: Правила защиты от потери данных для SSN не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308073"
---
Возникают проблемы с **Предотвращения потери данных (DLP)** не работает для контента, содержащий **Страховой номер (SSN)** при использовании тип конфиденциальных данных в Office 365? Если это так, убедитесь в том, что ваш контент содержит необходимые сведения для политики защиты от потери данных, которые выполняет поиск. 
  
Например для политики SSN, имеющей уровень вероятности 85%, следующие вычисляются и необходимо наличие для правила для запуска:
  
- **[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифр, которые могут быть в шаблоне форматированный или неформатированный 
    
- **[Шаблон:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четыре функции поиск SSNs в четыре разных шаблонов: 
    
  - Func_ssn находит SSN со строгим форматированием с тире или пробелами, выданные до 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);
    
  - Func_unformatted_ssn находит SSN со строгим форматированием, выданные до 2011 г. (без форматирования в виде девяти последовательных цифр — ццццццццц);
    
  - Func_randomized_formatted_ssn находит SSN с тире или пробелами, выданные после 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);
    
  - Func_randomized_unformatted_ssn находит SSN без форматирования в виде девяти последовательных цифр, выданные после 2011 г. (ццццццццц).
    
- **[Контрольная сумма:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Нет, не контрольной суммой 
    
- **[Определение:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Политика защиты от потери данных — это 85% уверены в том, что этот тип конфиденциальных данных обнаружил if в рамках близости 300 знаков: 
    
  - [Функция Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) находит контент, который соответствует шаблону. 
    
  - Ключевое слово из [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) найти. Включает в себя примеры ключевых слов: *социального страхования, социального страхования #, Soc сек, SSN* . Например, следующий пример приведет к запуску для политики защиты от потери данных SSN: **SSN: 489 36 8350**
    
Дополнительные сведения о что является необходимым для SSNs для обнаружения для содержимого в следующем разделе в этой статье: [Что конфиденциальные сведения типов искать SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
С помощью типа различных встроенных конфиденциальной информации, обратитесь к следующей статье сведения на что является необходимым для других типов: [Поиск что конфиденциальные сведения типов](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

