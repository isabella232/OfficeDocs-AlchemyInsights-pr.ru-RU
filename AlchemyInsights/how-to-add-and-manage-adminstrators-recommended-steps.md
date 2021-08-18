---
title: Добавление и управление администраторами — рекомендуемые действия
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339045"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Добавление и управление администраторами — рекомендуемые действия

На основе описания проблемы мы нашли решение для вас. Большинству клиентов удалось самостоятельно решить проблему после того, как мы высмеяли документацию.

**Изменение администратора подписки или со-администратора**

- Администратор учетной записи может изменять обе роли, в то время как администратор подписки может изменять со-администраторов только на [портале Azure.](https://ms.portal.azure.com/#home)
- [Добавление или изменение администраторов подписки Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Обновление администратора подписки или Co-Administrator для внутренних (AIRS) подписки**

Администратор службы или со-администратор могут самостоятельно обслуживать это действие, используя следующие действия:

1. Войдите на портал [Azure и](https://ms.portal.azure.com/#home) нажмите **кнопку Управление затратами и выставление счета** в левом лезвии.
2. Щелкните элемент строки с подпиской. Это открывает обзор подписки.
3. На **лезвии подписки** щелкните **Свойства**. 
4. Нажмите **кнопку Администрирование** службы.
5. Введите электронную почту пользователя, которого вы хотите настроить в качестве администратора службы, и нажмите **кнопку ОК.**

**Add/Change/Remove Co-administrator**

1. Войдите на портал [Azure в](https://ms.portal.azure.com/#home) качестве администратора службы.
2. Откройте [подписки](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) и выберите подписку. (Co-adminstrators can be assigned only at the subscription scope.)
3. Перейдите к классическим администраторам управления доступом **(IAM)** Добавьте со-администратора добавить, чтобы открыть области Добавить  >    >    >   **со-администратора** (Если параметр Добавить со-администратор отключен, это означает, что у вас нет разрешений).
4. Выберите пользователя, которого вы хотите добавить, и нажмите **кнопку Добавить**.

**Подробнее:**
- [Добавление со-администратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Удаление со-администратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Изменение администратора службы](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Просмотр администратора учетной записи](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Управление доступом с помощью портала RBAC и Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Добавление и удаление пользователей с Azure Active Directory (AD)**

Вы можете добавить новых пользователей или удалить существующие пользователи из Azure Active Directory организации Azure AD:

1. Чтобы добавить нового пользователя, войдите на портал [Azure](https://ms.portal.azure.com/#home) в качестве администратора пользователя для организации.
2. Выберите **Azure Active Directory,** выберите **Пользователей** и нажмите **кнопку Новый пользователь**.
3. На странице **Пользователь** заполните необходимые сведения. Нажмите кнопку **Создать**. Пользователь создается и добавляется в клиент Azure AD.

**Дополнительные**

- [Добавление нового пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Удаление пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Добавление или обновление сведений о профиле пользователя с помощью Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Рекомендуемые документы**

- [Что такое управление доступом на основе ролей (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Понимание различных ролей в Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Учебник. Предоставление доступа пользователю с помощью RBAC и портала Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Устранение неполадок RBAC в Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Организация ресурсов с помощью групп управления Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Запрос копии счета Azure по электронной почте](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Добавление, обновление или удаление кредитной или дебетовой карты из Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Подписка на управление (повторное включение/отмена/переключение)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



