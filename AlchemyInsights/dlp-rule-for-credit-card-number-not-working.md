---
title: Правила защиты от потери данных для номер кредитной карты не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657480"
---
Возникают проблемы с **Предотвращения потери данных (DLP)** не работает для контента, содержащий **Номер кредитной карты** , при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что ваш контент содержит необходимые сведения для запуска политики защиты от потери данных при вычислении ее. Например **данные о банковской карте политики** , настроенной с уровень вероятности 85%, следующие вычисляются и необходимо наличие для правила для запуска: 
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, которые могут иметь формат или неформатированные (dddddddddddddddd) и должно пройти проверку Luhn. 
    
- **[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Шаблон очень сложным и надежным, обнаруживает карты из всех основных торговых марок по всему миру, включая Visa, Mastercard, обнаружение карточки, JCB, American Express, подарочные сертификаты и diner карты. 
    
- **[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, контрольная сумма Luhn 
    
- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Политика защиты от потери данных — это 85% уверены в том, что этот тип конфиденциальных данных обнаружил if в рамках близости 300 знаков: 
    
  - Функция Func_credit_card находит содержимое, которое соответствует шаблону;
    
  - Верно одно из условий ниже: 
    
  - найдено ключевое слово из Keyword_cc_verification;
    
  - Найдено ключевого слова из Keyword_cc_name
    
  - функция Func_expiration_date находит дату в правильном формате.
    
  - Контрольная сумма передает
    
    Например следующий пример приведет к запуску для политики номер кредитной карты защиты от потери данных:
    
  - Visa: 7352 3952 3647 4485 
    
  - Действительно до: 2/2009 г.
    
Дополнительные сведения о что является необходимым для **Номер кредитной карты** для обнаружения для содержимого в следующем разделе в этой статье: [Что конфиденциальные сведения типов искать данные о банковской карте #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
С помощью типа различных встроенных конфиденциальной информации, обратитесь к следующей статье сведения на что является необходимым для других типов: [Поиск что конфиденциальные сведения типов](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

