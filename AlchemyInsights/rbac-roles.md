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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923144"
---
# <a name="rbac-rules"></a>Правила RBAC

Если вы получаете ошибку разрешения: 

- Клиент с объектным id не имеет разрешения на выполнение действий по области **(код: AuthorizationFailed)**: при попытке создания ресурса убедитесь, что вы в настоящее время подписаны с пользователем, на который назначена роль, которая имеет разрешение на написание ресурса в выбранной области. Например, для управления виртуальными машинами в группе [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) ресурсов необходимо иметь роль вкладчика виртуальных машин в группе ресурсов (или родительской области). Список разрешений для каждой встроенной роли см. в списке встроенных ролей [для ресурсов Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- У вас нет разрешения на создание запроса на поддержку: при попытке создания или обновления билета поддержки убедитесь, что вы в настоящее время подписаны с пользователем, который назначен роль, которая имеет microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Больше не могут создаваться назначения ролей **(код: RoleAssignmentLimitExceeded).** При попытке назначить роль попробуйте уменьшить количество назначений ролей, назначив роли группам. Azure поддерживает до **2000** назначений ролей на одну подписку.

Дополнительные сведения о ролях Azure RBAC см. в [материале Azure RBAC roles.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
