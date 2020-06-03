---
title: Правило DLP для номера кредитной карты не работает
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507419"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблемы с DLP с номерами кредитных карт

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблемы с DLP с номерами кредитных карт**

Проблемы с **предотвращением потери данных (DLP)** не работают для контента, содержащего **номер кредитной карты** , при использовании типа конфиденциальной информации DLP в O365? Если это так, убедитесь, что содержимое содержит необходимые сведения, чтобы активировать политику DLP при его оценке. Например, для **политики кредитных карт** , настроенной с уровнем вероятности 85%, оцениваются и должны быть обнаружены правила для активации правила:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифр, которые могут быть форматированными или неформатированными (цццццццццццццццц) и должны пройти проверку Луна.

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Очень сложный и надежный шаблон, который находит карты со всех основных торговых марок, включая Visa, MasterCard, обнаружение карт, JCB, американский Express, подарочные сертификаты и карточки Динер.

- **[Контрольная сумма:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Да, контрольная сумма Луна

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Политика защиты от потери данных — 85% уверенности в том, что этот тип конфиденциальной информации обнаружен, если в пределах расстояния от 300 символов:

  - Функция Func_credit_card находит содержимое, которое соответствует шаблону;

  - Верно одно из условий ниже:

  - найдено ключевое слово из Keyword_cc_verification;

  - Найдено ключевое слово из Keyword_cc_name

  - функция Func_expiration_date находит дату в правильном формате.

  - Контрольная сумма проходит

    Например, в приведенном ниже примере запускается политика номеров кредитных карт DLP.

  - Visa: 4485 3647 3952 7352
  
  - Срок действия: 2/2009

Дополнительные сведения о том, что требуется для обнаружения **номера кредитной карты** для контента, можно найти в следующем разделе этой статьи: [что представляют собой типы конфиденциальной информации для карты No](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Используя другой встроенный тип конфиденциальной информации, ознакомьтесь со следующей статьей, чтобы узнать, что необходимо для других типов: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  