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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600395"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="351ad-102">Выбытие средств прежних версий электронных данных</span><span class="sxs-lookup"><span data-stu-id="351ad-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="351ad-103">В результате новых и улучшенных функций обнаружения электронных данных в центре соответствия требованиям Microsoft 365 в ближайшие месяцы будут отменены следующие устаревшие средства обнаружения электронных данных и командлеты.</span><span class="sxs-lookup"><span data-stu-id="351ad-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="351ad-104">[Обнаружение электронных](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) данных на месте и [удержание на месте](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="351ad-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="351ad-105">Командлеты Exchange Online PowerShell, поддерживающие обнаружение электронных данных на месте и удержания на месте.</span><span class="sxs-lookup"><span data-stu-id="351ad-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="351ad-106">Эти командлеты обозначаются как командлеты \*-MailboxSearch. К ним относятся следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="351ad-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="351ad-107">New — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="351ad-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="351ad-108">Start — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="351ad-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="351ad-109">Stop — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="351ad-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="351ad-110">Set — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="351ad-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="351ad-111">Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="351ad-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="351ad-112">Следующие операции в API веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="351ad-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="351ad-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="351ad-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="351ad-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="351ad-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="351ad-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="351ad-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="351ad-116">Расширенное обнаружение электронных данных версии 1.0 для Office 365</span><span class="sxs-lookup"><span data-stu-id="351ad-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="351ad-117">**Временная шкала для выбытия**:</span><span class="sxs-lookup"><span data-stu-id="351ad-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="351ad-118">1 апреля 2020 г.: вы не сможете создавать новые операции поиска и удержания, но вы можете выполнять, редактировать и удалять существующие поисковые запросы на свой риск.</span><span class="sxs-lookup"><span data-stu-id="351ad-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="351ad-119">Служба поддержки Майкрософт больше не будет поддерживать & обнаружения электронных данных на месте в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="351ad-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="351ad-120">1 июля 2020 г.: & обнаружения электронных данных на месте хранит функции в центре администрирования Exchange, которые будут размещены в режиме только для чтения.</span><span class="sxs-lookup"><span data-stu-id="351ad-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="351ad-121">Это означает, что вы можете только удалять существующие поисковые запросы и удержания.</span><span class="sxs-lookup"><span data-stu-id="351ad-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="351ad-122">**Более подробную информацию можно узнать в**следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="351ad-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="351ad-123">Миграция поиска электронных данных прежних версий и удержаний в центре соответствия требованиям Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="351ad-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="351ad-124">Выбытие средств прежних версий электронных данных</span><span class="sxs-lookup"><span data-stu-id="351ad-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="351ad-125">Вопросы и ответы об обнаружении электронных данных на месте и удержания на месте</span><span class="sxs-lookup"><span data-stu-id="351ad-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



