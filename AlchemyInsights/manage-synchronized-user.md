---
title: Управление синхронизированным пользователем
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823980"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="703bb-102">Невозможно установить основной адрес электронной почты, изменить атрибуты пользователей или удалить или удалить синхронизированного пользователя</span><span class="sxs-lookup"><span data-stu-id="703bb-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="703bb-103">Если для среды включена синхронизация каталогов, некоторые атрибуты пользователя или объекта нельзя изменить с помощью центра администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="703bb-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="703bb-104">Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальные активные пользователи каталогов и консоль управления группами (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="703bb-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="703bb-105">Кроме того, можно изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью powershell, как показано в этих распространенных примерах:</span><span class="sxs-lookup"><span data-stu-id="703bb-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
