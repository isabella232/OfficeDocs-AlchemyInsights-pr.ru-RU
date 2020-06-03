---
title: Правило защиты от потери данных для SSN не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507383"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Проблемы с защитой от потери данных с номерами социального страхования

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблемы с DLP в службах SSNs**

Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер социального страхования (SSN)** при использовании типа конфиденциальной информации в Microsoft 365? Если это так, убедитесь, что содержимое содержит необходимые сведения о том, что делает политика защиты от потери данных. 
  
Например, для политики SSN, настроенной с уровнем вероятности 85%, оцениваются и должны обнаруживаться для триггера правила:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифр, которые могут относиться к форматированному или неформатированному шаблону

- **[Шаблон:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четыре функции ищут служб SSNs в четырех различных шаблонах:

  - Func_ssn находит SSN со строгим форматированием с тире или пробелами, выданные до 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);

  - Func_unformatted_ssn находит SSN со строгим форматированием, выданные до 2011 г. (без форматирования в виде девяти последовательных цифр — ццццццццц);

  - Func_randomized_formatted_ssn находит SSN с тире или пробелами, выданные после 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);

  - Func_randomized_unformatted_ssn находит SSN без форматирования в виде девяти последовательных цифр, выданные после 2011 г. (ццццццццц).

- **[Контрольная сумма:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Нет, контрольная сумма отсутствует

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Политика защиты от потери данных — 85% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:

  - [Функция Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) находит содержимое, которое соответствует шаблону;

  - Находится ключевое слово из [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn). К примерам ключевых слов относятся: *социальное страхование, социальное страхование #, SoC sec, SSN* . Например, следующий пример вызывает срабатывание политики SSN для защиты от потери данных: **SSN: 489-36-8350**
  
Дополнительные сведения о том, что требуется для обнаружения в службах Организации для контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для служб SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  