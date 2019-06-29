---
title: Правило защиты от потери данных для SSN не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389446"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Проблемы с защитой от потери данных с номерами социального страхования

Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер социального страхования (SSN)** при использовании типа конфиденциальной информации в Office 365? Если это так, убедитесь, что содержимое содержит необходимые сведения о том, что делает политика защиты от потери данных. 
  
Например, для политики SSN, настроенной с уровнем вероятности 85%, оцениваются и должны обнаруживаться для триггера правила:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифр, которые могут относиться к форматированному или неформатированному шаблону

- **[Шаблон:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четыре функции ищут служб SSNs в четырех различных шаблонах:

  - Func_ssn находит SSN со строгим форматированием с тире или пробелами, выданные до 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);

  - Func_unformatted_ssn находит SSN со строгим форматированием, выданные до 2011 г. (без форматирования в виде девяти последовательных цифр — ццццццццц);

  - Func_randomized_formatted_ssn находит SSN с тире или пробелами, выданные после 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);

  - Func_randomized_unformatted_ssn находит SSN без форматирования в виде девяти последовательных цифр, выданные после 2011 г. (ццццццццц).

- **[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Нет, контрольная сумма отсутствует

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Политика защиты от потери данных — 85% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:

  - [Функция функ_ссн](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) обнаружила содержимое, соответствующее шаблону.

  - Находится ключевое слово из [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn). К примерам ключевых слов относятся: *социальное страхование, социальное страхование #, SoC sec, SSN* . Например, следующий пример вызывает срабатывание политики SSN для защиты от потери данных: **SSN: 489-36-8350**
  
Дополнительные сведения о том, что требуется для обнаружения в службах Организации для контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для служб SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  