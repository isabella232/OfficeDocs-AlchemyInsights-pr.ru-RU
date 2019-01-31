---
title: Правила защиты от потери данных для "мне Нравится" номер банковского счета не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9fd5d4736c5209f85e235dc6a0846f65f1b5f624
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657012"
---
Возникают проблемы с **Предотвращения потери данных (DLP)** не работает для контента, содержащий **Номер банковского счета в США** , при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что ваш контент содержит необходимые сведения для что выполняет поиск политики защиты от потери данных при вычислении ее. 
  
К примеру для **Номер банковского счета США** политику, настроенную с уровень вероятности 85%, следующие вычисляются и необходимо наличие для правила для запуска: 
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифр 
    
- **[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 последовательных цифр. 
    
- **[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Нет, не контрольной суммой 
    
- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Политики защиты от потери данных — 75% уверены в том, что этот тип конфиденциальных данных обнаружил if в рамках близости 300 знаков: 
    
  - Находит контент, который соответствует шаблону регулярное выражение Regex_usa_bank_account_number
    
  - находится ключевое слово из Keyword_usa_Bank_Account.
    
    Например, следующий пример приведет к запуску для политики **Номер банковского счета США** : 78344011 счета 
    
Дополнительные сведения о что является необходимым для **США номер банковского счета** для обнаружения для содержимого в следующем разделе в этой статье: [Что конфиденциальные сведения типов искать номер банковского счета США.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
С помощью типа различных встроенных конфиденциальной информации, обратитесь к следующей статье сведения на что является необходимым для других типов: [Поиск что конфиденциальные сведения типов](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

