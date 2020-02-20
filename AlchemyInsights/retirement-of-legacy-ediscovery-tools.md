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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="badaf-102">Выбытие средств прежних версий электронных данных</span><span class="sxs-lookup"><span data-stu-id="badaf-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="badaf-103">В результате новых и улучшенных функций обнаружения электронных данных в центре соответствия требованиям Microsoft 365 в ближайшие месяцы будут отменены следующие устаревшие средства обнаружения электронных данных и командлеты.</span><span class="sxs-lookup"><span data-stu-id="badaf-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="badaf-104">[Обнаружение электронных](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) данных на месте и [удержание на месте](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="badaf-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="badaf-105">Командлеты Exchange Online PowerShell, поддерживающие обнаружение электронных данных на месте и удержания на месте.</span><span class="sxs-lookup"><span data-stu-id="badaf-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="badaf-106">Эти командлеты обозначаются как командлеты \*-MailboxSearch. К ним относятся следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="badaf-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="badaf-107">New — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="badaf-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="badaf-108">Start — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="badaf-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="badaf-109">Stop — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="badaf-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="badaf-110">Set — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="badaf-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="badaf-111">Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="badaf-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="badaf-112">Следующие операции в API веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="badaf-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="badaf-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="badaf-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="badaf-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="badaf-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="badaf-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="badaf-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="badaf-116">Расширенное обнаружение электронных данных версии 1.0 для Office 365</span><span class="sxs-lookup"><span data-stu-id="badaf-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="badaf-117">**Временная шкала для выбытия**:</span><span class="sxs-lookup"><span data-stu-id="badaf-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="badaf-118">1 апреля 2020 г.: вы не сможете создавать новые операции поиска и удержания, но вы можете выполнять, редактировать и удалять существующие поисковые запросы на свой риск.</span><span class="sxs-lookup"><span data-stu-id="badaf-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="badaf-119">Служба поддержки Майкрософт больше не будет поддерживать & обнаружения электронных данных на месте в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="badaf-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="badaf-120">1 июля 2020 г.: & обнаружения электронных данных на месте хранит функции в центре администрирования Exchange, которые будут размещены в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badaf-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="badaf-121">Это означает, что вы можете только удалять существующие поисковые запросы и удержания.</span><span class="sxs-lookup"><span data-stu-id="badaf-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="badaf-122">**Более подробную информацию можно узнать в**следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="badaf-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="badaf-123">Миграция поиска электронных данных прежних версий и удержаний в центре соответствия требованиям Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="badaf-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="badaf-124">Выбытие средств прежних версий электронных данных</span><span class="sxs-lookup"><span data-stu-id="badaf-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="badaf-125">Вопросы и ответы об обнаружении электронных данных на месте и удержания на месте</span><span class="sxs-lookup"><span data-stu-id="badaf-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



