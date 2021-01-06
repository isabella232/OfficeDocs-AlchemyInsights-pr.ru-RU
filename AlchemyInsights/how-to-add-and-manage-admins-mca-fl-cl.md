---
title: Добавление администраторов и управление ими
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755508"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="69a42-102">Добавление администраторов и управление ими</span><span class="sxs-lookup"><span data-stu-id="69a42-102">How to add and manage admins</span></span>

<span data-ttu-id="69a42-103">На основе описания проблемы мы нашли решение для вас.</span><span class="sxs-lookup"><span data-stu-id="69a42-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="69a42-104">Большинство клиентов смогли самостоятельно решить свою проблему после того, как мы сдали нашу документацию.</span><span class="sxs-lookup"><span data-stu-id="69a42-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="69a42-105">Для управления учетной записью вы выставления счетов в рамках соглашения с клиентом Майкрософт (MCA) можно использовать различные роли с нужным уровнем доступа.</span><span class="sxs-lookup"><span data-stu-id="69a42-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="69a42-106">Эти роли являются дополнением к встроенным ролям служб Azure, которые помогают управлять ресурсами.</span><span class="sxs-lookup"><span data-stu-id="69a42-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="69a42-107">**Добавление ролей вы выставления счета на портале Azure:**</span><span class="sxs-lookup"><span data-stu-id="69a42-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="69a42-108">Войдите на [портал Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="69a42-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="69a42-109">Выполните поиск по запросу *Управление затратами + выставление счетов*.</span><span class="sxs-lookup"><span data-stu-id="69a42-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="69a42-110">Выберите управление доступом (IAM) в области, такой как учетная запись выставления счетов, профиль выставления счетов или раздел счета, к которой вы хотите предоставить доступ.</span><span class="sxs-lookup"><span data-stu-id="69a42-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="69a42-111">На странице управления доступом (IAM) перечислены пользователи и группы, которые назначены каждой роли для этой области.</span><span class="sxs-lookup"><span data-stu-id="69a42-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="69a42-112">Чтобы предоставить доступ пользователю, выберите **"Добавить"** в верхней части страницы.</span><span class="sxs-lookup"><span data-stu-id="69a42-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="69a42-113">В *выпадаемом* списке ролей выберите роль.</span><span class="sxs-lookup"><span data-stu-id="69a42-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="69a42-114">Введите адрес электронной почты пользователя, к которому вы хотите предоставить доступ.</span><span class="sxs-lookup"><span data-stu-id="69a42-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="69a42-115">Чтобы назначить роль, нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="69a42-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="69a42-116">Чтобы удалить доступ для пользователя, выберите пользователя с назначением роли, которую необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="69a42-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="69a42-117">Выберите **"Удалить"**</span><span class="sxs-lookup"><span data-stu-id="69a42-117">Select **Remove**.</span></span>

<span data-ttu-id="69a42-118">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="69a42-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="69a42-119">Определения ролей вы выставления счета</span><span class="sxs-lookup"><span data-stu-id="69a42-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="69a42-120">Роли и задачи учетной записи вы выставления счетов</span><span class="sxs-lookup"><span data-stu-id="69a42-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="69a42-121">Начало работы с учетной записью для вычета MCA</span><span class="sxs-lookup"><span data-stu-id="69a42-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="69a42-122">Проверка доступа к соглашению с клиентом Майкрософт</span><span class="sxs-lookup"><span data-stu-id="69a42-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
