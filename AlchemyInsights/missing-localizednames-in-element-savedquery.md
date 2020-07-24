---
title: В элементе 'savedquery' отсутствует 'LocalizedNames'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1739"
- "9000187"
ms.openlocfilehash: a891b31e90951be8349a7fda705a14320e22fb3a
ms.sourcegitcommit: ebb3595422b581eca98a05533f8d82239daec09a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45207372"
---
# <a name="missing-localizednames-in-element-savedquery"></a><span data-ttu-id="27ebd-102">В элементе 'savedquery' отсутствует 'LocalizedNames'</span><span class="sxs-lookup"><span data-stu-id="27ebd-102">Missing 'LocalizedNames' in element 'savedquery'</span></span>

<span data-ttu-id="27ebd-103">Сведения о действиях в случае отсутствия 'LocalizedNames' см. в статье [При импорте решения Dynamics 365 возникает ошибка "Содержимое элемента 'savedquery' является неполным. Список ожидаемых элементов: 'LocalizedNames'"](https://support.microsoft.com/help/4463330/the-element-savedquery-has-incomplete-content-list-of-possible-element).</span><span class="sxs-lookup"><span data-stu-id="27ebd-103">For help with missing 'LocalizedNames', see ["The element 'savedquery' has incomplete content. List of possible elements expected: 'LocalizedNames'" error occurs when importing a Dynamics 365 solution](https://support.microsoft.com/help/4463330/the-element-savedquery-has-incomplete-content-list-of-possible-element).</span></span>

<span data-ttu-id="27ebd-104">Найдите специальные символы в имени представления, которые могут вызывать эту проблему.</span><span class="sxs-lookup"><span data-stu-id="27ebd-104">Look for special characters in the view name that might cause the issue.</span></span> <span data-ttu-id="27ebd-105">Удалите все специальные символы в имени представления и выполните экспорт решения повторно.</span><span class="sxs-lookup"><span data-stu-id="27ebd-105">Remove any special characters in the view name and export the solution again.</span></span>