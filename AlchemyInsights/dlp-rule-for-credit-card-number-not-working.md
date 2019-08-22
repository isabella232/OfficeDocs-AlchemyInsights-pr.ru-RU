---
title: Правило DLP для номера кредитной карты не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529968"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблемы с DLP с номерами кредитных карт

Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер кредитной карты** , при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что содержимое содержит необходимые сведения, чтобы активировать политику DLP при его оценке. Например, для **политики кредитных карт** , настроенной с уровнем вероятности 85%, оцениваются и должны быть обнаружены правила для активации правила:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифр, которые могут быть форматированными или неформатированными (цццццццццццццццц) и должны пройти проверку Луна.

- **[Шаблон:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Очень сложный и надежный шаблон, который находит карты со всех основных торговых марок, включая Visa, MasterCard, обнаружение карт, JCB, американский Express, подарочные сертификаты и карточки Динер.

- **[Контрольная сумма:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, контрольная сумма Луна

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Политика защиты от потери данных — 85% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:

  - Функция Func_credit_card находит содержимое, которое соответствует шаблону;

  - Верно одно из условий ниже:

  - найдено ключевое слово из Keyword_cc_verification;

  - Найдено ключевое слово из Keyword_cc_name

  - функция Func_expiration_date находит дату в правильном формате.

  - Контрольная сумма проходит

    Например, в приведенном ниже примере запускается политика номеров кредитных карт DLP.

  - Visa: 4485 3647 3952 7352
  
  - Срок действия: 2/2009

Дополнительные сведения о том, что требуется для обнаружения **номера кредитной карты** для контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для карты No](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  