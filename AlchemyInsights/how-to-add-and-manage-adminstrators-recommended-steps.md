---
title: Добавление администраторов и управление ими — рекомендуемые действия
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755848"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Добавление администраторов и управление ими — рекомендуемые действия

На основе описания проблемы мы нашли решение для вас. Большинство клиентов смогли самостоятельно решить свою проблему после того, как мы сдали нашу документацию.

**Изменение администратора подписки или со-администратора**

- Администратор учетных записей может редактировать обе роли, а администратор подписки — только на [портале Azure.](https://ms.portal.azure.com/#home)
- [Добавление или изменение администраторов подписки Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Обновление администратора или администратора Co-Administrator для внутренних подписок (AIRS)**

Администратор службы или со-администратор может самостоятельно выполнять это действие, вы используя следующие действия:

1. Войдите на портал [Azure и](https://ms.portal.azure.com/#home) щелкните "Управление затратами и выставление **счета"** в левой области.
2. Щелкните строку с подпиской. Откроется обзор подписки.
3. В blade **подписки** щелкните **"Свойства".** 
4. Нажмите **кнопку "Администратор** службы".
5. Введите сообщение электронной почты пользователя, которого вы хотите наметить администратором службы, и нажмите кнопку **"ОК".**

**Добавление, изменение и удаление со-администратора**

1. Войдите на портал [Azure с](https://ms.portal.azure.com/#home) учетной записью администратора службы.
2. Откройте [подписки](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) и выберите подписку. (Со-администраторы могут быть назначены только на уровне подписки.)
3. Перейдите к классическому администратору управления доступом **(IAM)** Добавление со-администратора для открытия области добавления со-администратора (если параметр "Добавить со-администратора" отключен, это означает, что у вас нет  >    >    >   разрешений). 
4. Выберите пользователя, которого вы хотите добавить, и нажмите кнопку **"Добавить".**

**Подробнее:**
- [Добавление со-администратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Удаление со-администратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Изменение администратора службы](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Просмотр администратора учетных записей](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Управление доступом с помощью RBAC и портала Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Добавление и удаление пользователей с помощью Azure Active Directory (AD)**

Вы можете добавлять новых или удалять существующих пользователей из своей организации Azure Active Directory (Azure AD):

1. Чтобы добавить нового пользователя, войдите на портал [Azure](https://ms.portal.azure.com/#home) с учетной записью администратора пользователя в организации.
2. Выберите **Azure Active Directory,** выберите **"Пользователи"** и нажмите кнопку **"Новый пользователь".**
3. На странице **"Пользователь"** заполните необходимые сведения. Нажмите кнопку **Создать**. Пользователь создается и добавляется в клиент Azure AD.

**Дополнительные узнайте:**

- [Добавление нового пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Удаление пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Добавление или обновление сведений профиля пользователя с помощью Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Рекомендуемые документы**

- [Что такое управление доступом на основе ролей (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Различные роли в Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Руководство. Предоставление доступа пользователю с помощью RBAC и портала Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Устранение неполадок RBAC в Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Организация ресурсов с помощью групп управления Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Как запросить копию счета-фактуры Azure по электронной почте](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Добавление, обновление или удаление кредитной или дебетовой карты из Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Управление подпиской (повторное включение, отмена и переключение)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



