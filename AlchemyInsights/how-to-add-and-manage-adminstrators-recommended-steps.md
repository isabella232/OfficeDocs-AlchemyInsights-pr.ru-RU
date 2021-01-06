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
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="2e973-102">Добавление администраторов и управление ими — рекомендуемые действия</span><span class="sxs-lookup"><span data-stu-id="2e973-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="2e973-103">На основе описания проблемы мы нашли решение для вас.</span><span class="sxs-lookup"><span data-stu-id="2e973-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="2e973-104">Большинство клиентов смогли самостоятельно решить свою проблему после того, как мы сдали нашу документацию.</span><span class="sxs-lookup"><span data-stu-id="2e973-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="2e973-105">**Изменение администратора подписки или со-администратора**</span><span class="sxs-lookup"><span data-stu-id="2e973-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="2e973-106">Администратор учетных записей может редактировать обе роли, а администратор подписки — только на [портале Azure.](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="2e973-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="2e973-107">Добавление или изменение администраторов подписки Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="2e973-108">**Обновление администратора или администратора Co-Administrator для внутренних подписок (AIRS)**</span><span class="sxs-lookup"><span data-stu-id="2e973-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="2e973-109">Администратор службы или со-администратор может самостоятельно выполнять это действие, вы используя следующие действия:</span><span class="sxs-lookup"><span data-stu-id="2e973-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="2e973-110">Войдите на портал [Azure и](https://ms.portal.azure.com/#home) щелкните "Управление затратами и выставление **счета"** в левой области.</span><span class="sxs-lookup"><span data-stu-id="2e973-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="2e973-111">Щелкните строку с подпиской.</span><span class="sxs-lookup"><span data-stu-id="2e973-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="2e973-112">Откроется обзор подписки.</span><span class="sxs-lookup"><span data-stu-id="2e973-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="2e973-113">В blade **подписки** щелкните **"Свойства".**</span><span class="sxs-lookup"><span data-stu-id="2e973-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="2e973-114">Нажмите **кнопку "Администратор** службы".</span><span class="sxs-lookup"><span data-stu-id="2e973-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="2e973-115">Введите сообщение электронной почты пользователя, которого вы хотите наметить администратором службы, и нажмите кнопку **"ОК".**</span><span class="sxs-lookup"><span data-stu-id="2e973-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="2e973-116">**Добавление, изменение и удаление со-администратора**</span><span class="sxs-lookup"><span data-stu-id="2e973-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="2e973-117">Войдите на портал [Azure с](https://ms.portal.azure.com/#home) учетной записью администратора службы.</span><span class="sxs-lookup"><span data-stu-id="2e973-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="2e973-118">Откройте [подписки](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) и выберите подписку.</span><span class="sxs-lookup"><span data-stu-id="2e973-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="2e973-119">(Со-администраторы могут быть назначены только на уровне подписки.)</span><span class="sxs-lookup"><span data-stu-id="2e973-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="2e973-120">Перейдите к классическому администратору управления доступом **(IAM)** Добавление со-администратора для открытия области добавления со-администратора (если параметр "Добавить со-администратора" отключен, это означает, что у вас нет  >    >    >   разрешений). </span><span class="sxs-lookup"><span data-stu-id="2e973-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="2e973-121">Выберите пользователя, которого вы хотите добавить, и нажмите кнопку **"Добавить".**</span><span class="sxs-lookup"><span data-stu-id="2e973-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="2e973-122">**Подробнее:**</span><span class="sxs-lookup"><span data-stu-id="2e973-122">**Learn more:**</span></span>
- [<span data-ttu-id="2e973-123">Добавление со-администратора</span><span class="sxs-lookup"><span data-stu-id="2e973-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2e973-124">Удаление со-администратора</span><span class="sxs-lookup"><span data-stu-id="2e973-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2e973-125">Изменение администратора службы</span><span class="sxs-lookup"><span data-stu-id="2e973-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2e973-126">Просмотр администратора учетных записей</span><span class="sxs-lookup"><span data-stu-id="2e973-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="2e973-127">Управление доступом с помощью RBAC и портала Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="2e973-128">**Добавление и удаление пользователей с помощью Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="2e973-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="2e973-129">Вы можете добавлять новых или удалять существующих пользователей из своей организации Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="2e973-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="2e973-130">Чтобы добавить нового пользователя, войдите на портал [Azure](https://ms.portal.azure.com/#home) с учетной записью администратора пользователя в организации.</span><span class="sxs-lookup"><span data-stu-id="2e973-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="2e973-131">Выберите **Azure Active Directory,** выберите **"Пользователи"** и нажмите кнопку **"Новый пользователь".**</span><span class="sxs-lookup"><span data-stu-id="2e973-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="2e973-132">На странице **"Пользователь"** заполните необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="2e973-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="2e973-133">Нажмите кнопку **Создать**.</span><span class="sxs-lookup"><span data-stu-id="2e973-133">Click **Create**.</span></span> <span data-ttu-id="2e973-134">Пользователь создается и добавляется в клиент Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2e973-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="2e973-135">**Дополнительные узнайте:**</span><span class="sxs-lookup"><span data-stu-id="2e973-135">**Learn more**:</span></span>

- [<span data-ttu-id="2e973-136">Добавление нового пользователя</span><span class="sxs-lookup"><span data-stu-id="2e973-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="2e973-137">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="2e973-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="2e973-138">Добавление или обновление сведений профиля пользователя с помощью Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2e973-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="2e973-139">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="2e973-139">**Recommended documents**</span></span>

- [<span data-ttu-id="2e973-140">Что такое управление доступом на основе ролей (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="2e973-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="2e973-141">Различные роли в Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="2e973-142">Разрешения роли администратора в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2e973-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="2e973-143">Руководство. Предоставление доступа пользователю с помощью RBAC и портала Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="2e973-144">Устранение неполадок RBAC в Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="2e973-145">Организация ресурсов с помощью групп управления Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="2e973-146">Как запросить копию счета-фактуры Azure по электронной почте</span><span class="sxs-lookup"><span data-stu-id="2e973-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="2e973-147">Добавление, обновление или удаление кредитной или дебетовой карты из Azure</span><span class="sxs-lookup"><span data-stu-id="2e973-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="2e973-148">Управление подпиской (повторное включение, отмена и переключение)</span><span class="sxs-lookup"><span data-stu-id="2e973-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



