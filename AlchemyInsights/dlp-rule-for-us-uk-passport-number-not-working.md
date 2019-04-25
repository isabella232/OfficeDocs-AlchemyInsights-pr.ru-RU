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
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблемы с номерами паспорта DLP-US/Великобритании

Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер паспорта США/Великобритании** при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь в том, что содержимое содержит необходимые сведения о том, какие параметры политики DLP ищет при оценке. 
  
Например, для политики **номера паспорта США и Великобритании** , настроенной на уровне вероятности 75%, оцениваются и должны быть обнаружены для правила, которое необходимо активировать 
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девять цифр 
    
- **[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девять последовательных цифр 
    
- **[КонтрольНая сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Нет, контрольная сумма отсутствует 
    
- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Политика защиты от потери данных — 75% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов: 
    
  - функция Func_usa_uk_passport находит содержимое, которое соответствует шаблону;
    
  - находится ключевое слово из Keyword_passport.
    
    Например, следующий пример вызывает срабатывание политики **номеров паспортов для США и Великобритании** : номер паспорта США 123456789 
    
Дополнительные сведения о том, что требуется для обнаружения номера паспорта US/Великобритании для вашего контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальНой информации для номера паспорта США и Великобритании](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальНой информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

