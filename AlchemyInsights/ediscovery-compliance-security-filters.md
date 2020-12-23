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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727236"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="f2746-102">Результаты поиска и экспорта контента не возвращаются</span><span class="sxs-lookup"><span data-stu-id="f2746-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="f2746-103">Если у вас возникли проблемы со следующими сценариями eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="f2746-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="f2746-104">Поиск и экспорт контента не возвращают данных или непредвиденных данных</span><span class="sxs-lookup"><span data-stu-id="f2746-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="f2746-105">Не удается найти или экспортировать eDiscovery</span><span class="sxs-lookup"><span data-stu-id="f2746-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="f2746-106">Это может быть вызвано определенными фильтрами безопасности соответствия требованиям, которые были настроены определенным администратором и не были оадминистрироваться всем администраторам.</span><span class="sxs-lookup"><span data-stu-id="f2746-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="f2746-107">Чтобы устранить эту проблему, проверьте, есть ли фильтры соответствия требованиям безопасности, которые могут быть причиной таких проблем:</span><span class="sxs-lookup"><span data-stu-id="f2746-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="f2746-108">Подключение к Powershell Центра безопасности и соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="f2746-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="f2746-109">Запустите следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="f2746-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="f2746-110">Дополнительные сведения о фильтрах безопасности соответствия требованиям см. в подкассылной области ["Фильтрация разрешений для поиска контента"](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="f2746-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
