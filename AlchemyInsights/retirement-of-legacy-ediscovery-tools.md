---
title: Выбытие средств прежних версий электронных данных
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157692"
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

- [Расширенное обнаружение электронных данных версии 1.0 для Office 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Временная шкала для выбытия**:
- 1 апреля 2020 г.: вы не сможете создавать новые операции поиска и удержания, но вы можете выполнять, редактировать и удалять существующие поисковые запросы на свой риск. Служба поддержки Майкрософт больше не будет поддерживать & обнаружения электронных данных на месте в центре администрирования Exchange.

- 1 июля 2020 г.: & обнаружения электронных данных на месте хранит функции в центре администрирования Exchange, которые будут размещены в режиме только для чтения. Это означает, что вы можете только удалять существующие поисковые запросы и удержания.

**Более подробную информацию можно узнать в**следующих статьях:

 - [Миграция поиска электронных данных прежних версий и удержаний в центре соответствия требованиям Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Выбытие средств прежних версий электронных данных](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Вопросы и ответы об обнаружении электронных данных на месте и удержания на месте](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



