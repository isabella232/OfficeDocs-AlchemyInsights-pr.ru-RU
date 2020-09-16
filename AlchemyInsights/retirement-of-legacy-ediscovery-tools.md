---
title: Выбытие средств прежних версий электронных данных
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727796"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Выбытие средств прежних версий электронных данных

В результате новых и улучшенных функций обнаружения электронных данных в центре соответствия требованиям Microsoft 365 в ближайшие месяцы будут отменены следующие устаревшие средства обнаружения электронных данных и командлеты.

- [Обнаружение электронных](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) данных на месте и [удержание на месте](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центре администрирования Exchange.

- Командлеты Exchange Online PowerShell, поддерживающие обнаружение электронных данных на месте и удержания на месте. Эти командлеты обозначаются как командлеты *-MailboxSearch. К ним относятся следующие командлеты:

    - [New — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.
- Следующие операции в API веб-служб Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Расширенное обнаружение электронных данных v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Временная шкала для выбытия**:
- **1 июля 2020 г** . Вы больше не можете создавать новые поисковые запросы и удержания, но можете запускать, редактировать и удалять существующие поисковые запросы на свой риск. Служба поддержки Майкрософт больше не поддерживает & обнаружения электронных данных на месте в центре администрирования Exchange.
    
- **1 октября 2020 г** . & обнаружения электронных данных на месте: функции в центре администрирования Exchange будут размещены в режиме только для чтения, поэтому вы можете удалять только существующие запросы поиска и удержания.

**Более подробную информацию можно узнать в**следующих статьях:

 - [Миграция поиска электронных данных прежних версий и удержаний в центре соответствия требованиям Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Прекращение поддержки устаревших средств обнаружения электронных данных](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Вопросы и ответы об обнаружении электронных данных на месте и удержания на месте](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



