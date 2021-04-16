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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798562"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Выход на пенсию устаревших средств для электронных обнаружений

В результате новых и улучшенных функций по обнаружению электронных данных в центре соответствия требованиям Microsoft 365 следующие устаревшие средства и командные команды электронной почты будут отправлены в отставку в ближайшие месяцы:

- [Открытие электронных данных на месте](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) и удерживает на месте [в](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) центре администрирования Exchange.

- Комлеты Exchange Online PowerShell, которые поддерживают In-Place и In-Place удерживает. (Эти cmdlets совместно определены как *-MailboxSearch cmdlets.) Это включает в себя следующие cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Комлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.
- Следующие операции в API веб-служб Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Сроки выхода на пенсию:**
- **1 июля 2020 г.** Вы больше не можете создавать новые поиски и удерживает, но вы можете запускать, редактировать и удалять существующие поиски на свой собственный риск. Поддержка Майкрософт больше не поддерживает In-Place электронных & в EAC.
    
- **1 октября 2020** In-Place функции & eDiscovery в EAC будут размещены в режиме только для чтения, поэтому можно удалить только существующие поиски и удерживает.

**Дополнительные сведения см. в .**

 - [Перенос устаревших поисков электронных данных и их перенос в центр соответствия требованиям Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Прекращение поддержки устаревших средств обнаружения электронных данных](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQs about In-Place eDiscovery and In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



