---
title: Предоставление разрешений
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897757"
---
# <a name="grant-permissions"></a><span data-ttu-id="ee9e3-102">Предоставление разрешений</span><span class="sxs-lookup"><span data-stu-id="ee9e3-102">Grant permissions</span></span>

1. <span data-ttu-id="ee9e3-103">Предоставление согласия администратора для [](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) всего **клиента.** Пошаговые инструкции по предоставлению согласия администратора для всего клиента на портале Azure, с помощью Azure AD PowerShell или самого запроса согласия администратора см. в этой теме.</span><span class="sxs-lookup"><span data-stu-id="ee9e3-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="ee9e3-104">**Предоставление** согласия от имени определенного пользователя: вместо предоставления согласия для всей организации администратор также может использовать [API Microsoft Graph](https://docs.microsoft.com/graph/use-the-api) для предоставления согласия на делегирование разрешений от имени одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ee9e3-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="ee9e3-105">Дополнительные сведения см. в сведениях о том, как получить доступ [от имени пользователя.](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="ee9e3-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>