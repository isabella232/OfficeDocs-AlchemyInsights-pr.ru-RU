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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542015"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="9ef8c-102">Не удается задать основной адрес электронной почты или изменить атрибуты пользователя</span><span class="sxs-lookup"><span data-stu-id="9ef8c-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="9ef8c-103">Если для вашей среды включена синхронизация службы каталогов, некоторые атрибуты пользователя или объекта невозможно изменить с помощью центра администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ef8c-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="9ef8c-104">Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальную консоль управления пользователями и группами Active Directory (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="9ef8c-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="9ef8c-105">Кроме того, вы можете изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью PowerShell, как показано в следующих примерах:</span><span class="sxs-lookup"><span data-stu-id="9ef8c-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="9ef8c-106">Set – MsolUser — UserPrincipalName user@yourdomain.onmicrosoft.com — Алтернатимаиладдрессес user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9ef8c-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="9ef8c-107">Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"</span><span class="sxs-lookup"><span data-stu-id="9ef8c-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="9ef8c-108">Remove — MsolUser — UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9ef8c-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>