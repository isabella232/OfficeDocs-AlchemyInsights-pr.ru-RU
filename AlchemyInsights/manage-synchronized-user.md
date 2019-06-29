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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380518"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="14c6c-102">Не удается задать основной адрес электронной почты или изменить атрибуты пользователя</span><span class="sxs-lookup"><span data-stu-id="14c6c-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="14c6c-103">Если для вашей среды включена синхронизация службы каталогов, некоторые атрибуты пользователя или объекта невозможно изменить с помощью центра администрирования.</span><span class="sxs-lookup"><span data-stu-id="14c6c-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="14c6c-104">Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальную консоль управления пользователями и группами Active Directory (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="14c6c-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="14c6c-105">Кроме того, вы можете изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью PowerShell, как показано в следующих примерах:</span><span class="sxs-lookup"><span data-stu-id="14c6c-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="14c6c-106">Set – MsolUser — UserPrincipalName user@yourdomain.onmicrosoft.com — Алтернатимаиладдрессес user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="14c6c-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="14c6c-107">Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"</span><span class="sxs-lookup"><span data-stu-id="14c6c-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="14c6c-108">Remove — MsolUser — UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="14c6c-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>