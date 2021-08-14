---
title: Правило DLP для номера кредитной карты не работает
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005103"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблемы с DLP с номерами кредитных карт

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблемы с DLP с номерами кредитных карт**

Возникают ли проблемы с предотвращением потери данных **(DLP),** не работающим с контентом, содержащим номер кредитной карты при использовании типа конфиденциальной информации DLP в O365?  Если это так, убедитесь, что содержимое содержит необходимые сведения для запуска политики DLP при ее оценке. Например, для  политики кредитных карт, настроенной с уровнем уверенности в 85%, оцениваются следующие правила, которые должны быть обнаружены для запуска правила:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифр, которые могут быть отформатированы или неформатированы (dddd) и должны пройти тест Luhn.

- **[Шаблон:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Очень сложный и надежный шаблон, который обнаруживает карты всех крупных брендов по всему миру, включая карты Visa, MasterCard, Discover Card, JCB, American Express, подарочные карты и карточки для посетителей.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Да, проверки Luhn

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Политика DLP на 85% уверена в том, что она обнаруживает этот тип конфиденциальной информации, если в непосредственной близости от 300 символов:

  - Функция Func_credit_card находит содержимое, которое соответствует шаблону;

  - Верно одно из условий ниже:

  - найдено ключевое слово из Keyword_cc_verification;

  - Ключевое слово из Keyword_cc_name найдено

  - функция Func_expiration_date находит дату в правильном формате.

  - Проходит проверка

    Например, в следующем примере запускается политика номеров кредитных карт DLP:

  - Виза: 4485 3647 3952 7352
  
  - Срок действия: 2/2009

Дополнительные сведения о том,  что требуется для обнаружения номера кредитной карты для контента, см. в следующем [разделе.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
С помощью другого встроенного типа конфиденциальной информации см. в следующей статье сведения о том, что требуется для других [типов.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  