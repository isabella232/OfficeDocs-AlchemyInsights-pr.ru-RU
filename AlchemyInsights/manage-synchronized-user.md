---
title: Управление синхронизированным пользователем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407363"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="6a125-102">Не удается задать основной адрес электронной почты, изменить атрибуты пользователя, удалить или удалить синхронизированного пользователя</span><span class="sxs-lookup"><span data-stu-id="6a125-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="6a125-103">Если для вашей среды включена синхронизация службы каталогов, некоторые атрибуты пользователя или объекта невозможно изменить с помощью центра администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a125-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="6a125-104">Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальную консоль управления пользователями и группами Active Directory (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="6a125-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="6a125-105">Кроме того, вы можете изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью PowerShell, как показано в следующих примерах:</span><span class="sxs-lookup"><span data-stu-id="6a125-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
