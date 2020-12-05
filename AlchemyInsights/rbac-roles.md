---
title: 'Роли RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576625"
---
# <a name="rbac-rules"></a><span data-ttu-id="1d3e1-102">Правила RBAC</span><span class="sxs-lookup"><span data-stu-id="1d3e1-102">RBAC rules</span></span>

<span data-ttu-id="1d3e1-103">Если возникнет ошибка разрешения:</span><span class="sxs-lookup"><span data-stu-id="1d3e1-103">If you get the permission error:</span></span> 

- <span data-ttu-id="1d3e1-104">**Клиент с идентификатором объекта не имеет авторизации для выполнения действий с областью действия (Code: аусоризатионфаилед)**: при попытке создать ресурс убедитесь, что вход выполнен с помощью пользователя, которому назначена роль, имеющая разрешение на запись для ресурса в выбранной области.</span><span class="sxs-lookup"><span data-stu-id="1d3e1-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="1d3e1-105">Например, чтобы управлять виртуальными машинами в группе ресурсов, у вас должна быть роль [участника виртуальной машины](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в группе ресурсов (или родительской области).</span><span class="sxs-lookup"><span data-stu-id="1d3e1-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="1d3e1-106">Список разрешений для каждой встроенной роли вы найдете в статье [встроенные роли для ресурсов Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1d3e1-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="1d3e1-107">У **вас нет разрешения на создание запроса на поддержку**: при попытке создать или обновить билет в службу поддержки убедитесь, что вы выполнили вход с учетной записью пользователя, которому назначена роль с разрешениями Microsoft. support/суппорттиккетс/Write, например [участник запроса поддержки](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="1d3e1-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="1d3e1-108">Больше **не удается создать назначения ролей (код: ролеассигнментлимитексцеедед)**: при попытке назначить роль уменьшите число назначений ролей, назначая роли группам.</span><span class="sxs-lookup"><span data-stu-id="1d3e1-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="1d3e1-109">Azure поддерживает до **2000** назначений ролей для каждой подписки.</span><span class="sxs-lookup"><span data-stu-id="1d3e1-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="1d3e1-110">Дополнительные сведения о ролях Azure RBAC приведены в статье [роли Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1d3e1-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
