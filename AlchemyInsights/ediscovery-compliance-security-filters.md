---
title: Результаты поиска и экспорта контента не возвращаются
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666653"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="87353-102">Результаты поиска и экспорта контента не возвращаются</span><span class="sxs-lookup"><span data-stu-id="87353-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="87353-103">Если у вас возникли проблемы со следующими сценариями eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="87353-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="87353-104">Поиск и экспорт контента не возвращают данных или непредвиденных данных</span><span class="sxs-lookup"><span data-stu-id="87353-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="87353-105">Не удается найти или экспортировать eDiscovery</span><span class="sxs-lookup"><span data-stu-id="87353-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="87353-106">Это может быть вызвано определенными фильтрами безопасности соответствия требованиям, которые были настроены определенным администратором и не были донесы до всех администраторов.</span><span class="sxs-lookup"><span data-stu-id="87353-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="87353-107">Чтобы устранить эту проблему, проверьте, есть ли какие-либо фильтры соответствия требованиям безопасности, которые могут быть причиной таких проблем:</span><span class="sxs-lookup"><span data-stu-id="87353-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="87353-108">Подключение к Powershell Центра безопасности и соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="87353-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="87353-109">Запустите следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="87353-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="87353-110">Дополнительные сведения о фильтрах безопасности соответствия требованиям см. в фильтрации разрешений [для поиска контента](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="87353-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
