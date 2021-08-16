---
title: Правило DLP для номера паспортов США и Великобритании не работает
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004959"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблемы с DLP - номера паспортов США и Великобритании

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблемы с номерами паспортов США и Великобритании**

Возникли ли проблемы с предотвращением потери данных **(DLP),** не работающим с контентом, содержащим номер паспорта США **и** Великобритании при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что содержимое содержит необходимые сведения о том, что ищет политика DLP при оценке.
  
Например, для политики номеров паспортов США **и** Великобритании, настроенной с уровнем доверия 75%, для запуска правила необходимо определить следующие данные.
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Девять цифр

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Девять последовательных цифр

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Нет, нет checksum

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Политика DLP на 75% уверена, что она обнаруживает этот тип конфиденциальной информации, если в непосредственной близости от 300 символов:

  - функция Func_usa_uk_passport находит содержимое, которое соответствует шаблону;

  - находится ключевое слово из Keyword_passport.

    Например, в следующем примере  срабатывает политика номеров паспортов США и Великобритании: номер 123456789

Дополнительные сведения о том, что требуется для обнаружения номера паспорта США и Великобритании для вашего контента, см. в следующем [разделе.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
С помощью другого встроенного типа конфиденциальной информации см. в следующей статье сведения о том, что требуется для других [типов.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  