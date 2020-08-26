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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902633"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="46bfd-102">Выбытие средств прежних версий электронных данных</span><span class="sxs-lookup"><span data-stu-id="46bfd-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="46bfd-103">В результате новых и улучшенных функций обнаружения электронных данных в центре соответствия требованиям Microsoft 365 в ближайшие месяцы будут отменены следующие устаревшие средства обнаружения электронных данных и командлеты.</span><span class="sxs-lookup"><span data-stu-id="46bfd-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="46bfd-104">[Обнаружение электронных](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) данных на месте и [удержание на месте](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="46bfd-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="46bfd-105">Командлеты Exchange Online PowerShell, поддерживающие обнаружение электронных данных на месте и удержания на месте.</span><span class="sxs-lookup"><span data-stu-id="46bfd-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="46bfd-106">Эти командлеты обозначаются как командлеты \*-MailboxSearch. К ним относятся следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="46bfd-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="46bfd-107">New — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="46bfd-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="46bfd-108">Start — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="46bfd-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="46bfd-109">Stop — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="46bfd-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="46bfd-110">Set — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="46bfd-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="46bfd-111">Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="46bfd-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="46bfd-112">Следующие операции в API веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="46bfd-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="46bfd-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="46bfd-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="46bfd-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="46bfd-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="46bfd-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="46bfd-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="46bfd-116">Расширенное обнаружение электронных данных v 1.0</span><span class="sxs-lookup"><span data-stu-id="46bfd-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="46bfd-117">**Временная шкала для выбытия**:</span><span class="sxs-lookup"><span data-stu-id="46bfd-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="46bfd-118">**1 июля 2020 г** . Вы больше не можете создавать новые поисковые запросы и удержания, но можете запускать, редактировать и удалять существующие поисковые запросы на свой риск.</span><span class="sxs-lookup"><span data-stu-id="46bfd-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="46bfd-119">Служба поддержки Майкрософт больше не поддерживает & обнаружения электронных данных на месте в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="46bfd-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="46bfd-120">**1 октября 2020 г** . & обнаружения электронных данных на месте: функции в центре администрирования Exchange будут размещены в режиме только для чтения, поэтому вы можете удалять только существующие запросы поиска и удержания.</span><span class="sxs-lookup"><span data-stu-id="46bfd-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="46bfd-121">**Более подробную информацию можно узнать в**следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="46bfd-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="46bfd-122">Миграция поиска электронных данных прежних версий и удержаний в центре соответствия требованиям Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="46bfd-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="46bfd-123">Прекращение поддержки устаревших средств обнаружения электронных данных</span><span class="sxs-lookup"><span data-stu-id="46bfd-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="46bfd-124">Вопросы и ответы об обнаружении электронных данных на месте и удержания на месте</span><span class="sxs-lookup"><span data-stu-id="46bfd-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



