---
title: Правило защиты от потери данных для номера банковского счета США не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977175"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Проблемы с DLP с номерами банковских счетов США

**Важно!** в это незначительное время мы предоставим вам рекомендации по включению служб SharePoint Online и OneDrive, чтобы получить дополнительные сведения о [временных функциях SharePoint](https://aka.ms/ODSPAdjustments) Online.

**Проблемы с DLP с номерами банковских счетов США**

Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер банковского счета США** при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь в том, что содержимое содержит необходимые сведения о том, какие параметры политики DLP ищет при оценке.
  
Например, для политики **номеров банковских счетов США** , настроенной на уровне вероятности 85%, оцениваются и должны быть обнаружены правила для активации правила:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифр

- **[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 последовательных цифр.

- **[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Нет, контрольная сумма отсутствует

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Политика защиты от потери данных — 75% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:

  - Регулярное выражение Regex_usa_bank_account_number находит содержимое, которое соответствует шаблону;

  - находится ключевое слово из Keyword_usa_Bank_Account.

    Например, следующий пример вызывает срабатывание политики **номеров банковских счетов США** : Проверка учетной записи 78344011

Дополнительные сведения о том, что требуется для обнаружения **номера банковского счета США** , можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для банковского счета США](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  