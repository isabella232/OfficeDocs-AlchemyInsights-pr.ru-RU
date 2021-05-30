---
title: Микрозадержки или регулирование скорости в Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702139"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="2f825-102">Микрозадержки или регулирование скорости в Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="2f825-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="2f825-103">При запуске сценариев и командлетов в Exchange Online могут отображаться предупреждения "Применена микрозадержка" или возникать задержки.</span><span class="sxs-lookup"><span data-stu-id="2f825-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="2f825-104">Вот несколько советов по решению этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="2f825-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="2f825-105">Запустите наше средство диагностики, чтобы сделать политику регулирования PowerShell на вашем клиенте менее жесткой.</span><span class="sxs-lookup"><span data-stu-id="2f825-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="2f825-106">Это решает проблему в большинстве случаев.</span><span class="sxs-lookup"><span data-stu-id="2f825-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="2f825-107">Если проблема не исчезнет, попробуйте использовать [модуль PowerShell Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true): он включает командлеты на основе API REST, их производительность значительно выше.</span><span class="sxs-lookup"><span data-stu-id="2f825-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="2f825-108">Это решение может быть оптимальным для множества часто используемых командлетов Get.</span><span class="sxs-lookup"><span data-stu-id="2f825-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="2f825-109">Если нужно использовать командлеты, не входящие в состав модуля v2, см статью [Запуск командлетов PowerShell для большого количества пользователей в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#). В ней описываются обходные решения для ограничений регулирования PowerShell в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2f825-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
