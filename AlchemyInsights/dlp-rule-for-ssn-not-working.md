---
title: Правило DLP для SSN не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004995"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Проблемы DLP с номерами социального страхования

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблемы DLP с SSNs**

Возникают ли проблемы с предотвращением потери данных **(DLP),** не работающим с контентом, содержащим номер социального обеспечения **(SSN)** при использовании типа конфиденциальной информации в Microsoft 365? Если это так, убедитесь, что содержимое содержит необходимые сведения для политики DLP. 
  
Например, для политики SSN, настроенной с уровнем доверия в 85%, оцениваются следующие правила, которые должны быть обнаружены для запуска правила:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифр, которые могут быть в форматированном или неформатированном шаблоне

- **[Шаблон:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четыре функции искать SSNs в четырех различных шаблонов:

  - Func_ssn находит SSN со строгим форматированием с тире или пробелами, выданные до 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);

  - Func_unformatted_ssn находит SSN со строгим форматированием, выданные до 2011 г. (без форматирования в виде девяти последовательных цифр — ццццццццц);

  - Func_randomized_formatted_ssn находит SSN с тире или пробелами, выданные после 2011 г. (ццц-цц-цццц ИЛИ ццц цц цццц);

  - Func_randomized_unformatted_ssn находит SSN без форматирования в виде девяти последовательных цифр, выданные после 2011 г. (ццццццццц).

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Нет, нет checksum

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Политика DLP на 85% уверена в том, что она обнаруживает этот тип конфиденциальной информации, если в непосредственной близости от 300 символов:

  - Функция [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) контента, который соответствует шаблону.

  - Находится ключевое слово из [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn). Примеры ключевых слов: социальное  *обеспечение, социальное обеспечение #, Soc Sec , SSN*  . Например, следующий пример запускает политику SSN DLP: **SSN: 489-36-8350**
  
Дополнительные сведения о том, что требуется для обнаружения SSNs для контента, см. в следующем [разделе.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
С помощью другого встроенного типа конфиденциальной информации см. в следующей статье сведения о том, что требуется для других [типов.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  