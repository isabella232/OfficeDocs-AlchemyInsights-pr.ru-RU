---
title: Один пользователь не видит надстройки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154575"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="3558d-102">Один пользователь не видит надстройки в Outlook</span><span class="sxs-lookup"><span data-stu-id="3558d-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="3558d-103">Возможно, пользователь является частью роли, содержащей неправильный параметр AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="3558d-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="3558d-104">Чтобы узнать, связана ли с пользователем правильная роль, запустите этот командлет:</span><span class="sxs-lookup"><span data-stu-id="3558d-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="3558d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="3558d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="3558d-106">Дополнительные сведения см. в статье [Выбор администраторов и пользователей, которые могут устанавливать надстройки для Outlook и управлять ими](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="3558d-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
