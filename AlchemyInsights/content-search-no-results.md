---
title: Поиск контента без результатов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680660"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="36d16-102">Нет результатов из поиска и экспортов контента</span><span class="sxs-lookup"><span data-stu-id="36d16-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="36d16-103">Проблемы с поиском контента и экспортами не возвращают данные могут быть вызваны определенным администратором и не взаимодействующими со всеми администраторами.</span><span class="sxs-lookup"><span data-stu-id="36d16-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="36d16-104">Чтобы устранить эту проблему, проверьте наличие фильтров безопасности соответствия, которые могут привести к этому.</span><span class="sxs-lookup"><span data-stu-id="36d16-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="36d16-105">Подключение к PowerShell центра безопасности и соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="36d16-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="36d16-106">Выполните следующую команду командлеты:</span><span class="sxs-lookup"><span data-stu-id="36d16-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="36d16-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="36d16-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="36d16-108">Get – ComplianceSecurityFilter — организация $org</span><span class="sxs-lookup"><span data-stu-id="36d16-108">Get-ComplianceSecurityFilter -Organization $org</span></span>