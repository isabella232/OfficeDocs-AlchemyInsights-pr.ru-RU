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
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656436"
---
Возникают проблемы с **Предотвращения потери данных (DLP)** не работает контента, содержащий **США / номер паспорта (Великобритания)** при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что ваш контент содержит необходимые сведения для что выполняет поиск политики защиты от потери данных при вычислении ее. 
  
Например, для **США / номер паспорта (Великобритания)** политику, настроенную с уровень вероятности 75%, перечисленные ниже вычисляются и необходимо наличие для правила для запуска 
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девяти цифр 
    
- **[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девять последовательных цифр 
    
- **[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Нет, не контрольной суммой 
    
- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Политики защиты от потери данных — 75% уверены в том, что этот тип конфиденциальных данных обнаружил if в рамках близости 300 знаков: 
    
  - функция Func_usa_uk_passport находит содержимое, которое соответствует шаблону;
    
  - находится ключевое слово из Keyword_passport.
    
    Например, следующий пример приведет к запуску для **США / номер паспорта (Великобритания)** политики: номер паспорта США 123456789 
    
Для получения дополнительных сведений о что является необходимым для США / номер паспорта (Великобритания) для обнаружения для содержимого, в следующем разделе в этой статье: [что конфиденциальные сведения типов внешнего вида для США / номер паспорта (Великобритания)](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
С помощью типа различных встроенных конфиденциальной информации, обратитесь к следующей статье сведения на что является необходимым для других типов: [Поиск что конфиденциальные сведения типов](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

