---
title: Добавление и Управление Администраторы — Рекомендуемые действия
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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599518"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Добавление и Управление Администраторы — Рекомендуемые действия

**Изменение администратора подписки или соадминистратора**

- Администратор учетной записи может изменять обе роли, а администратор подписки может изменять только соадминистраторами на [портале Azure](https://ms.portal.azure.com/#home).
- [Добавление или изменение администраторов Подписки Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Обновление администратора подписки или Co-Administrator для подписок на внутренние (трансляции) подписки**

Администратор службы или Соадминистратор может самостоятельно выполнить это действие, выполнив следующие действия:

1. Войдите на [портал Azure](https://ms.portal.azure.com/#home) и выберите **Управление затратами + выставление счетов** в левом колонке.
2. Щелкните элемент Line с подпиской. Откроется Обзор подписки.
3. В колонке **Подписка** нажмите кнопку **свойства**. 
4. Нажмите кнопку **администратор службы** .
5. Введите адрес электронной почты пользователя, которого вы хотите назначить администратором службы, и нажмите кнопку **ОК**.

**Добавление, изменение и удаление соадминистратора**

1. Войдите на [портал Azure](https://ms.portal.azure.com/#home) с учетной записью администратора службы.
2. Откройте [подписку и](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) выберите подписку. (Co-администраторы можно назначить только в области подписки.)
3. Перейдите к классическим администраторам **управления доступом (IAM)**  >  **Classic administrators**  >  **Добавить**  >  **Добавить соадминистратора** , чтобы открыть область **Добавить** совместный доступ (если параметр Добавить Соадминистратор отключен, он указывает, что у вас нет разрешений).
4. Выберите пользователя, которого нужно добавить, и нажмите кнопку **Добавить**.

**Подробнее:**
- [Добавление соадминистратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Удаление соадминистратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Изменение администратора службы](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Просмотр администратора учетных записей](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Управление доступом с помощью RBAC и портала Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Добавление и удаление пользователей с помощью Azure Active Directory (AD)**

Вы можете добавлять новых пользователей или удалять существующих пользователей из вашей организации Azure Active Directory (Azure AD):

1. Чтобы добавить нового пользователя, войдите на [портал Azure](https://ms.portal.azure.com/#home) с учетной записью администратора в Организации.
2. Выберите **Azure Active Directory**, выберите **Пользователи** , а затем щелкните **Новый пользователь**.
3. На странице **User (пользователь** ) заполните необходимые сведения. Нажмите **Создать**. Пользователь создается и добавляется в клиент Azure AD.

Дополнительные **сведения**:

- [Добавление нового пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Удаление пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Добавление или обновление сведений о профиле пользователя с помощью Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Рекомендуемые документы**

- [Что такое управление доступом на основе ролей (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Общие сведения о различных ролях в Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Руководство: предоставление доступа для пользователя с помощью RBAC и портала Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Устранение неполадок RBAC в Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Организация ресурсов с помощью групп управления Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Запрос копии счета Azure через электронную почту](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Добавление, обновление или удаление кредитной или дебетовой карты в Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Управление подпиской (повторная активация/отмена/переключение)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



