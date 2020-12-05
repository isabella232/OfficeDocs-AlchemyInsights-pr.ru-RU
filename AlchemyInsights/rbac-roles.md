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
# <a name="rbac-rules"></a>Правила RBAC

Если возникнет ошибка разрешения: 

- **Клиент с идентификатором объекта не имеет авторизации для выполнения действий с областью действия (Code: аусоризатионфаилед)**: при попытке создать ресурс убедитесь, что вход выполнен с помощью пользователя, которому назначена роль, имеющая разрешение на запись для ресурса в выбранной области. Например, чтобы управлять виртуальными машинами в группе ресурсов, у вас должна быть роль [участника виртуальной машины](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в группе ресурсов (или родительской области). Список разрешений для каждой встроенной роли вы найдете в статье [встроенные роли для ресурсов Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- У **вас нет разрешения на создание запроса на поддержку**: при попытке создать или обновить билет в службу поддержки убедитесь, что вы выполнили вход с учетной записью пользователя, которому назначена роль с разрешениями Microsoft. support/суппорттиккетс/Write, например [участник запроса поддержки](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Больше **не удается создать назначения ролей (код: ролеассигнментлимитексцеедед)**: при попытке назначить роль уменьшите число назначений ролей, назначая роли группам. Azure поддерживает до **2000** назначений ролей для каждой подписки.

Дополнительные сведения о ролях Azure RBAC приведены в статье [роли Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
