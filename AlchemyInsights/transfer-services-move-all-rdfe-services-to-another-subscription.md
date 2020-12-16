---
title: Службы переноса — перемещение всех служб RDFE в другую подписку
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681479"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="52af1-102">Службы переноса — перемещение всех служб RDFE в другую подписку</span><span class="sxs-lookup"><span data-stu-id="52af1-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="52af1-103">**Перемещение ресурсов**</span><span class="sxs-lookup"><span data-stu-id="52af1-103">**Move resources**</span></span>

<span data-ttu-id="52af1-104">Ресурсы Azure можно переместить в другую подписку Azure или группу ресурсов по той же подписке с помощью портала Azure, Azure PowerShell, Azure CLI или REST API для перемещения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="52af1-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="52af1-105">Перед перемещением ресурсов см. статью:</span><span class="sxs-lookup"><span data-stu-id="52af1-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="52af1-106">Контрольный список перед перемещением ресурсов</span><span class="sxs-lookup"><span data-stu-id="52af1-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="52af1-107">Службы, которые можно перемещать</span><span class="sxs-lookup"><span data-stu-id="52af1-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="52af1-108">Проверка перемещения</span><span class="sxs-lookup"><span data-stu-id="52af1-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="52af1-109">Руководство по переходу на службы</span><span class="sxs-lookup"><span data-stu-id="52af1-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="52af1-110">Чтобы переместить существующие ресурсы в другую группу ресурсов или подписку, можно использовать:</span><span class="sxs-lookup"><span data-stu-id="52af1-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="52af1-111">Портал Azure</span><span class="sxs-lookup"><span data-stu-id="52af1-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="52af1-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="52af1-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="52af1-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="52af1-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="52af1-114">REST API</span><span class="sxs-lookup"><span data-stu-id="52af1-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="52af1-115">Руководство. [Перемещение ресурсов Azure в другую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="52af1-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="52af1-116">**Устранение ошибок с помощью Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="52af1-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="52af1-117">Сведения о некоторых распространенных ошибках развертывания Azure и их устранении см. в статьях ниже.</span><span class="sxs-lookup"><span data-stu-id="52af1-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="52af1-118">Если код ошибки развертывания не найти, см. статью ["Поиск кода ошибки".](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)</span><span class="sxs-lookup"><span data-stu-id="52af1-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="52af1-119">Устранение ошибок развертывания</span><span class="sxs-lookup"><span data-stu-id="52af1-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="52af1-120">Устранение неполадок при перемещении ресурсов Azure в новую группу ресурсов или подписку</span><span class="sxs-lookup"><span data-stu-id="52af1-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="52af1-121">Обратите внимание, что если вы хотите обновить подписку Azure, например перейти с бесплатной на оплату по мере необходимости, вам потребуется преобразовать подписку.</span><span class="sxs-lookup"><span data-stu-id="52af1-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="52af1-122">Чтобы обновить бесплатную пробную подписку, см. обновление бесплатной пробной подписки [или подписки Microsoft Imagine Azure до оплаты](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)по мере использования.</span><span class="sxs-lookup"><span data-stu-id="52af1-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="52af1-123">Чтобы изменить счет с оплатой по мере использования, см. подписку [на Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)на другое предложение.</span><span class="sxs-lookup"><span data-stu-id="52af1-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="52af1-124">**Чтобы добавить или связать подписку Azure с клиентом Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="52af1-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="52af1-125">Во sign in and select the subscription you want to use from the [Subscriptions page in Azure portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="52af1-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="52af1-126">Выберите **"Изменить каталог".**</span><span class="sxs-lookup"><span data-stu-id="52af1-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="52af1-127">Просмотрите все появляющиеся предупреждения и выберите **"Изменить".**</span><span class="sxs-lookup"><span data-stu-id="52af1-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="52af1-128">Каталог для подписки изменен, и вы получите сообщение об успешном результате.</span><span class="sxs-lookup"><span data-stu-id="52af1-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="52af1-129">Используйте *переключатель каталогов,* чтобы перейти в новый каталог.</span><span class="sxs-lookup"><span data-stu-id="52af1-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="52af1-130">Для правильного показа всего может потребоваться до 10 минут.</span><span class="sxs-lookup"><span data-stu-id="52af1-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="52af1-131">**Рекомендуемые документы**</span><span class="sxs-lookup"><span data-stu-id="52af1-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="52af1-132">Передача прав владельца подписки Azure</span><span class="sxs-lookup"><span data-stu-id="52af1-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="52af1-133">Перемещение ресурсов в новую группу ресурсов или подписку</span><span class="sxs-lookup"><span data-stu-id="52af1-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="52af1-134">Управление ресурсами с помощью портала Azure</span><span class="sxs-lookup"><span data-stu-id="52af1-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
