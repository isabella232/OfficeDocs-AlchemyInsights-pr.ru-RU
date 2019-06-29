---
title: 929 правила для папки "Входящие" Дефлекттранспорт
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6cf996e6d0a2698a5ce2bb57251de7c61d248d2a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382678"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="3938d-102">Правила для поток обработки почты (также называемые правилами транспорта)</span><span class="sxs-lookup"><span data-stu-id="3938d-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="3938d-103">Общие сведения о правилах для поток обработки почты: [правила для поток обработки почты (правила транспорта) в Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="3938d-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="3938d-104">Настройка правил для почтового процесса: [процедуры правил обработки почты в Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="3938d-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="3938d-105">Создание, изменение и удаление правил для процесса обработки почты: [Управление правилами обработки почты](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="3938d-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="3938d-106">Вы также можете управлять правилами обработки почты в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3938d-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="3938d-107">Дополнительные сведения см. в статье [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (View) [, New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Create), Remove [-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (Modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (Disable existing) и [Enable — TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (включить существующие).</span><span class="sxs-lookup"><span data-stu-id="3938d-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="3938d-108">Дополнительные командлеты правил обработки почты: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (список доступных действий), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (список доступных условий и исключений), [Export-транспортрулеколлектион](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (правила экспорта) и [ Import-Транспортрулеколлектион](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (правила импорта).</span><span class="sxs-lookup"><span data-stu-id="3938d-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
