---
title: Поиск контента без результатов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516792"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="9463c-102">Нет результатов из поиска и экспортов контента</span><span class="sxs-lookup"><span data-stu-id="9463c-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="9463c-103">Проблемы с поиском контента и экспортами не возвращают данные могут быть вызваны определенным администратором и не взаимодействующими со всеми администраторами.</span><span class="sxs-lookup"><span data-stu-id="9463c-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="9463c-104">Чтобы устранить эту проблему, проверьте наличие фильтров безопасности соответствия, которые могут привести к этому.</span><span class="sxs-lookup"><span data-stu-id="9463c-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="9463c-105">Подключение к PowerShell центра безопасности и соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="9463c-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="9463c-106">Выполните следующую команду командлеты:</span><span class="sxs-lookup"><span data-stu-id="9463c-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="9463c-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="9463c-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="9463c-108">Get – ComplianceSecurityFilter — организация $org</span><span class="sxs-lookup"><span data-stu-id="9463c-108">Get-ComplianceSecurityFilter -Organization $org</span></span>