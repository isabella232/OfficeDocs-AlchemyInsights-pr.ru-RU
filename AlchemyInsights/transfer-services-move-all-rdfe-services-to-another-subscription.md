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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Службы переноса — перемещение всех служб RDFE в другую подписку

**Перемещение ресурсов**

Ресурсы Azure можно переместить в другую подписку Azure или группу ресурсов по той же подписке с помощью портала Azure, Azure PowerShell, Azure CLI или REST API для перемещения ресурсов.

Перед перемещением ресурсов см. статью:

- [Контрольный список перед перемещением ресурсов](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Службы, которые можно перемещать](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Проверка перемещения](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Руководство по переходу на службы](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Чтобы переместить существующие ресурсы в другую группу ресурсов или подписку, можно использовать:

- [Портал Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Руководство. [Перемещение ресурсов Azure в другую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Устранение ошибок с помощью Azure Resource Manager**

Сведения о некоторых распространенных ошибках развертывания Azure и их устранении см. в статьях ниже. Если код ошибки развертывания не найти, см. статью ["Поиск кода ошибки".](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Устранение ошибок развертывания](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Устранение неполадок при перемещении ресурсов Azure в новую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Обратите внимание, что если вы хотите обновить подписку Azure, например перейти с бесплатной на оплату по мере необходимости, вам потребуется преобразовать подписку.

- Чтобы обновить бесплатную пробную подписку, см. обновление бесплатной пробной подписки [или подписки Microsoft Imagine Azure до оплаты](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)по мере использования.
- Чтобы изменить счет с оплатой по мере использования, см. подписку [на Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)на другое предложение.

**Чтобы добавить или связать подписку Azure с клиентом Azure Active Directory:**

1. Во sign in and select the subscription you want to use from the [Subscriptions page in Azure portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Выберите **"Изменить каталог".**
3. Просмотрите все появляющиеся предупреждения и выберите **"Изменить".**
4. Каталог для подписки изменен, и вы получите сообщение об успешном результате.
5. Используйте *переключатель каталогов,* чтобы перейти в новый каталог. Для правильного показа всего может потребоваться до 10 минут.

**Рекомендуемые документы**

- [Передача прав владельца подписки Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Перемещение ресурсов в новую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Управление ресурсами с помощью портала Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
