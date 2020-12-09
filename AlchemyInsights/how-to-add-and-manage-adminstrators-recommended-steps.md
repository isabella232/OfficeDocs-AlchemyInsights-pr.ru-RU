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
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="7b6a8-102">Добавление и Управление Администраторы — Рекомендуемые действия</span><span class="sxs-lookup"><span data-stu-id="7b6a8-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="7b6a8-103">**Изменение администратора подписки или соадминистратора**</span><span class="sxs-lookup"><span data-stu-id="7b6a8-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="7b6a8-104">Администратор учетной записи может изменять обе роли, а администратор подписки может изменять только соадминистраторами на [портале Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="7b6a8-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="7b6a8-105">Добавление или изменение администраторов Подписки Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="7b6a8-106">**Обновление администратора подписки или Co-Administrator для подписок на внутренние (трансляции) подписки**</span><span class="sxs-lookup"><span data-stu-id="7b6a8-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="7b6a8-107">Администратор службы или Соадминистратор может самостоятельно выполнить это действие, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7b6a8-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="7b6a8-108">Войдите на [портал Azure](https://ms.portal.azure.com/#home) и выберите **Управление затратами + выставление счетов** в левом колонке.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="7b6a8-109">Щелкните элемент Line с подпиской.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="7b6a8-110">Откроется Обзор подписки.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="7b6a8-111">В колонке **Подписка** нажмите кнопку **свойства**.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="7b6a8-112">Нажмите кнопку **администратор службы** .</span><span class="sxs-lookup"><span data-stu-id="7b6a8-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="7b6a8-113">Введите адрес электронной почты пользователя, которого вы хотите назначить администратором службы, и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="7b6a8-114">**Добавление, изменение и удаление соадминистратора**</span><span class="sxs-lookup"><span data-stu-id="7b6a8-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="7b6a8-115">Войдите на [портал Azure](https://ms.portal.azure.com/#home) с учетной записью администратора службы.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="7b6a8-116">Откройте [подписку и](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) выберите подписку.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="7b6a8-117">(Co-администраторы можно назначить только в области подписки.)</span><span class="sxs-lookup"><span data-stu-id="7b6a8-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="7b6a8-118">Перейдите к классическим администраторам **управления доступом (IAM)**  >  **Classic administrators**  >  **Добавить**  >  **Добавить соадминистратора** , чтобы открыть область **Добавить** совместный доступ (если параметр Добавить Соадминистратор отключен, он указывает, что у вас нет разрешений).</span><span class="sxs-lookup"><span data-stu-id="7b6a8-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="7b6a8-119">Выберите пользователя, которого нужно добавить, и нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="7b6a8-120">**Подробнее:**</span><span class="sxs-lookup"><span data-stu-id="7b6a8-120">**Learn more:**</span></span>
- [<span data-ttu-id="7b6a8-121">Добавление соадминистратора</span><span class="sxs-lookup"><span data-stu-id="7b6a8-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7b6a8-122">Удаление соадминистратора</span><span class="sxs-lookup"><span data-stu-id="7b6a8-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7b6a8-123">Изменение администратора службы</span><span class="sxs-lookup"><span data-stu-id="7b6a8-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7b6a8-124">Просмотр администратора учетных записей</span><span class="sxs-lookup"><span data-stu-id="7b6a8-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="7b6a8-125">Управление доступом с помощью RBAC и портала Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="7b6a8-126">**Добавление и удаление пользователей с помощью Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="7b6a8-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="7b6a8-127">Вы можете добавлять новых пользователей или удалять существующих пользователей из вашей организации Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="7b6a8-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="7b6a8-128">Чтобы добавить нового пользователя, войдите на [портал Azure](https://ms.portal.azure.com/#home) с учетной записью администратора в Организации.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="7b6a8-129">Выберите **Azure Active Directory**, выберите **Пользователи** , а затем щелкните **Новый пользователь**.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="7b6a8-130">На странице **User (пользователь** ) заполните необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="7b6a8-131">Нажмите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-131">Click **Create**.</span></span> <span data-ttu-id="7b6a8-132">Пользователь создается и добавляется в клиент Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7b6a8-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="7b6a8-133">Дополнительные **сведения**:</span><span class="sxs-lookup"><span data-stu-id="7b6a8-133">**Learn more**:</span></span>

- [<span data-ttu-id="7b6a8-134">Добавление нового пользователя</span><span class="sxs-lookup"><span data-stu-id="7b6a8-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="7b6a8-135">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="7b6a8-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="7b6a8-136">Добавление или обновление сведений о профиле пользователя с помощью Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7b6a8-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="7b6a8-137">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="7b6a8-137">**Recommended documents**</span></span>

- [<span data-ttu-id="7b6a8-138">Что такое управление доступом на основе ролей (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="7b6a8-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="7b6a8-139">Общие сведения о различных ролях в Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="7b6a8-140">Разрешения роли администратора в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7b6a8-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="7b6a8-141">Руководство: предоставление доступа для пользователя с помощью RBAC и портала Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="7b6a8-142">Устранение неполадок RBAC в Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="7b6a8-143">Организация ресурсов с помощью групп управления Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="7b6a8-144">Запрос копии счета Azure через электронную почту</span><span class="sxs-lookup"><span data-stu-id="7b6a8-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="7b6a8-145">Добавление, обновление или удаление кредитной или дебетовой карты в Azure</span><span class="sxs-lookup"><span data-stu-id="7b6a8-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="7b6a8-146">Управление подпиской (повторная активация/отмена/переключение)</span><span class="sxs-lookup"><span data-stu-id="7b6a8-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



