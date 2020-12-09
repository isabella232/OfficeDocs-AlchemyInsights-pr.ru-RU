---
title: Включение управления затратами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599083"
---
# <a name="enable-cost-management"></a><span data-ttu-id="bf3de-102">Включение управления затратами</span><span class="sxs-lookup"><span data-stu-id="bf3de-102">Enable cost management</span></span>

<span data-ttu-id="bf3de-103">**Что означает, что затраты для вашей организации отключены?**</span><span class="sxs-lookup"><span data-stu-id="bf3de-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="bf3de-104">Организации, использующие учетные записи с корпоративным соглашением (EA) или Microsoft Customer Agreement (MCA), могут отключить доступ к сведениям о затратах и ценах.</span><span class="sxs-lookup"><span data-stu-id="bf3de-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="bf3de-105">После входа на портал Azure они могут использовать API выставления счетов для программного получения накладных (после выбора) и сведений об использовании.</span><span class="sxs-lookup"><span data-stu-id="bf3de-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="bf3de-106">**Как разрешить дополнительным пользователям получать доступ к счетам**</span><span class="sxs-lookup"><span data-stu-id="bf3de-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="bf3de-107">Перейдите к **колонке подписки** на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bf3de-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="bf3de-108">Выберите **счета** , а затем **доступ к счетам**.</span><span class="sxs-lookup"><span data-stu-id="bf3de-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="bf3de-109">Включите доступ, а затем сохраните изменения, чтобы разрешить пользователям в ролях с уровнями подписки загружать накладные.</span><span class="sxs-lookup"><span data-stu-id="bf3de-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="bf3de-110">Администратор учетной записи также может настроить для выставления счетов, отправляемых через электронную почту.</span><span class="sxs-lookup"><span data-stu-id="bf3de-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="bf3de-111">Чтобы узнать больше, ознакомьтесь со [статьей получение счета по электронной почте](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="bf3de-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="bf3de-112">**Добавление пользователей в роль читателя выставления счетов**</span><span class="sxs-lookup"><span data-stu-id="bf3de-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="bf3de-113">Перейдите к **колонке подписки** на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bf3de-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="bf3de-114">Выберите **Управление доступом (IAM)** , а затем нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="bf3de-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="bf3de-115">Выберите **средство "читатель выставления счетов** " на странице " **Выбор роли** ".</span><span class="sxs-lookup"><span data-stu-id="bf3de-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="bf3de-116">Введите адрес электронной почты пользователя, которого требуется пригласить, а затем нажмите кнопку **ОК** , чтобы отправить приглашение.</span><span class="sxs-lookup"><span data-stu-id="bf3de-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="bf3de-117">Следуйте инструкциям, приведенным в разделе приглашение, для входа в качестве средства чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="bf3de-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="bf3de-118">Для получения дополнительных сведений обратитесь [к разделу предоставление доступа для выставления счетов](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="bf3de-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="bf3de-119">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="bf3de-119">**Recommended documents**</span></span>

- [<span data-ttu-id="bf3de-120">Включение представлений DA и АО с помощью портала EA</span><span class="sxs-lookup"><span data-stu-id="bf3de-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="bf3de-121">Затраты, включенные в управление затратами</span><span class="sxs-lookup"><span data-stu-id="bf3de-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="bf3de-122">Поддерживаемые предложения Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="bf3de-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="bf3de-123">Просмотр затрат в анализе затрат</span><span class="sxs-lookup"><span data-stu-id="bf3de-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="bf3de-124">Предоставление доступа к сведениям о выставлении счетов</span><span class="sxs-lookup"><span data-stu-id="bf3de-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bf3de-125">Проверка доступа к соглашению о клиентах корпорации Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bf3de-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






