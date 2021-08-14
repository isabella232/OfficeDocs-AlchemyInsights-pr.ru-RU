---
title: Правило DLP для номера банковских счетов США не работает
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005031"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Проблемы с DLP с номерами банковских счетов США

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблемы с DLP с номерами банковских счетов США**

Возникли ли проблемы с предотвращением потери данных **(DLP),** не работающим с контентом, содержащим номер учетной записи банка США при использовании типа конфиденциальной информации DLP в O365?  Если это так, убедитесь, что содержимое содержит необходимые сведения о том, что ищет политика DLP при оценке.
  
Например, для  политики номеров банковских счетов США, настроенной с уровнем доверия в 85%, для запуска правила необходимо определить следующее:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифр

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 последовательных цифр.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Нет, нет checksum

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Политика DLP на 75% уверена, что она обнаруживает этот тип конфиденциальной информации, если в непосредственной близости от 300 символов:

  - Регулярное выражение Regex_usa_bank_account_number находит содержимое, которое соответствует шаблону

  - находится ключевое слово из Keyword_usa_Bank_Account.

    Например, в следующем примере  срабатывает политика номеров банковских счетов США: Проверка 78344011

Дополнительные сведения о том,  что требуется для обнаружения номера банковского счета в США для контента, см. в следующем [разделе.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
С помощью другого встроенного типа конфиденциальной информации см. в следующей статье сведения о том, что требуется для других [типов.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  