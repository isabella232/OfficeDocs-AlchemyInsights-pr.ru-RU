---
title: Передача прав владения на выставление счетов Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840634"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="c6304-102">Передача прав владения на выставление счетов Azure</span><span class="sxs-lookup"><span data-stu-id="c6304-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="c6304-103">Войдите на [портал Azure](https://portal.azure.com/) в качестве администратора учетной записи по выставлению счетов, содержащей подписку, которую вы хотите передать.</span><span class="sxs-lookup"><span data-stu-id="c6304-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="c6304-104">Если вы не знаете, являетесь ли вы администратором или вам нужно определить, кто является администратором, см. раздел [Определение администратора выставления счетов для учетной записи](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="c6304-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="c6304-105">Выполните поиск по запросу **Управление затратами + выставление счетов**.</span><span class="sxs-lookup"><span data-stu-id="c6304-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="c6304-106">Выберите **Подписки** в области слева.</span><span class="sxs-lookup"><span data-stu-id="c6304-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="c6304-107">В зависимости от уровня доступа вам может потребоваться выбрать область выставления счетов, а затем нажать **Подписки** или **Подписки Azure**.</span><span class="sxs-lookup"><span data-stu-id="c6304-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="c6304-108">Выберите **Передать права владения на выставление счетов** для подписки, которую хотите передать.</span><span class="sxs-lookup"><span data-stu-id="c6304-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="c6304-109">Введите адрес электронной почты пользователя, который является администратором выставления счетов для учетной записи, которая станет новым владельцем подписки, а затем выберите пункт **Отправить запрос на передачу**</span><span class="sxs-lookup"><span data-stu-id="c6304-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="c6304-110">Пользователь получит сообщение электронной почты с инструкциями по проверке вашего запроса на передачу.</span><span class="sxs-lookup"><span data-stu-id="c6304-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="c6304-111">Чтобы утвердить запрос на передачу, пользователь выбирает ссылку в сообщении электронной почты и следует инструкциям.</span><span class="sxs-lookup"><span data-stu-id="c6304-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="c6304-112">**Примечание**. Если вы передаете права владения на выставление счетов учетной записи пользователя в другом клиенте Azure AD, все назначения по [управлению доступом на основе ролей (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для управления ресурсами в подписке безвозвратно удаляются.</span><span class="sxs-lookup"><span data-stu-id="c6304-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="c6304-113">Доступ к управлению ресурсами в подписке будет иметь только новый владелец.</span><span class="sxs-lookup"><span data-stu-id="c6304-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="c6304-114">Дополнительные сведения см. в статье [Передача подписки пользователю в другом клиенте Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c6304-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c6304-115">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="c6304-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="c6304-116">Передача прав владения на выставление счетов подписки Azure в другую учетную запись</span><span class="sxs-lookup"><span data-stu-id="c6304-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="c6304-117">Сведения о передаче прав владения на выставление счетов для подписки Azure</span><span class="sxs-lookup"><span data-stu-id="c6304-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="c6304-118">Передача подписок на разработку и тестирование с оплатой по мере использования в среде Visual Studio, Microsoft Partner Network (MPN)</span><span class="sxs-lookup"><span data-stu-id="c6304-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="c6304-119">Вопросы и ответы о передаче прав владения</span><span class="sxs-lookup"><span data-stu-id="c6304-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="c6304-120">Устранение проблем при передаче прав владения</span><span class="sxs-lookup"><span data-stu-id="c6304-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
