---
title: Устранение ошибок с удержаниями при обнаружении электронных данных
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583761"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="74579-102">Устранение ошибок с удержаниями при обнаружении электронных данных</span><span class="sxs-lookup"><span data-stu-id="74579-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="74579-103">Возникли проблемы с удержаниями при обнаружении электронных данных?</span><span class="sxs-lookup"><span data-stu-id="74579-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="74579-104">Вот некоторые рекомендации:</span><span class="sxs-lookup"><span data-stu-id="74579-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="74579-105">Проверьте состояние распространения удержания.</span><span class="sxs-lookup"><span data-stu-id="74579-105">Check the hold distribution status.</span></span>  <span data-ttu-id="74579-106">Если отображается состояние **Включено (ожидание)** или **Отключено (ожидание)**, дождись завершения распространения удержания.</span><span class="sxs-lookup"><span data-stu-id="74579-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="74579-107">Объединяйте обновления удержаний при обнаружении электронных данных в один массовый запрос вместо многократного обновления политики для каждой транзакции.</span><span class="sxs-lookup"><span data-stu-id="74579-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="74579-108">Запустите Set-CaseHoldPolicy <policyname> -RetryDistribution в PowerShell Центра безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="74579-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="74579-109">Подробные сведения см. в статье [Подключение к оболочке PowerShell Центра безопасности и соответствия требованиям](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="74579-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="74579-110">Инструкции по проверке этих параметров и дополнительные рекомендации по устранению проблем с удержаниями при обнаружении электронных данных см. в статье [Устранение ошибок с удержаниями при обнаружении электронных данных](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="74579-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="74579-111">Сведения об устранении других распространенных проблем с обнаружением электронных данных см. в статье [Исследование, устранение неполадок и исправление распространенных проблем с обнаружением электронных данных](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="74579-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
