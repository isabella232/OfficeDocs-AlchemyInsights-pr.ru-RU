---
title: Выход на пенсию устаревших средств для электронных обнаружений
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074687"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Выход на пенсию устаревших средств для электронных обнаружений

В результате новых и улучшенных функций по обнаружению электронных данных в центре Microsoft 365 соответствия требованиям в ближайшие месяцы будут отменены следующие устаревшие средства и командные команды eDiscovery:

- [Открытие электронных данных](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) месте и удерживает на месте в центре Exchange администрирования.

- Эти Exchange Online PowerShell, которые поддерживают In-Place и In-Place удерживает. (Эти cmdlets совместно определены как *-MailboxSearch cmdlets.) Это включает в себя следующие cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Комлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.
- Следующие операции в API Exchange веб-служб:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Сроки выхода на пенсию:**
- **1 июля 2020 г.** Вы больше не можете создавать новые поиски и удерживает, но вы можете запускать, редактировать и удалять существующие поиски на свой собственный риск. Поддержка Майкрософт больше не поддерживает In-Place электронных & в EAC.
    
- **1 октября 2020** In-Place функции & eDiscovery в EAC будут размещены в режиме только для чтения, поэтому можно удалить только существующие поиски и удерживает.

**Дополнительные сведения см. в .**

 - [Перенос устаревших поисков электронных поисков и удерживает их в Центр соответствия требованиям Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Прекращение поддержки устаревших средств обнаружения электронных данных](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQs about In-Place eDiscovery and In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



