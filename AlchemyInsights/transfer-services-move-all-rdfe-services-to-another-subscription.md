---
title: Службы передачи — перемещение всех служб RDFE в другую подписку
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940080"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Службы передачи — перемещение всех служб RDFE в другую подписку

**Перемещение ресурсов**

Ресурсы Azure можно переместить в другую подписку Azure или группу ресурсов по той же подписке с помощью портала Azure, Azure PowerShell, Azure CLI или API REST для перемещения ресурсов.

Перед перемещением ресурсов см.:

- [Контрольный список перед перемещением ресурсов](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Службы, которые могут быть перемещены](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Проверка перемещения](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Перемещение руководства по службам](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Чтобы переместить существующие ресурсы в другую группу ресурсов или подписку, можно использовать:

- [Портал Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Руководство. [Перемещение ресурсов Azure в другую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Устранение ошибок с помощью Azure Resource Manager**

Обратитесь к статьям ниже, чтобы узнать о некоторых распространенных ошибках развертывания Azure и получить сведения для их устранения. Если вы не можете найти код ошибки для ошибки развертывания, см. [в статью Найти код ошибки.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Устранение ошибок развертывания](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Устранение неполадок при перемещении ресурсов Azure в новую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Обратите внимание, что если вы хотите обновить подписку Azure, например перейти с бесплатной на платную, необходимо преобразовать подписку.

- Чтобы обновить бесплатную пробную версия, см. в журнале [Upgrade your Free Trial или Microsoft Imagine Azure подписку на Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Чтобы изменить учетную запись с оплатой по мере использования, см. в журнале [Change your Azure Pay-As-You-Go на другое предложение.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Чтобы добавить или связать подписку Azure с Azure Active Directory клиентом:**

1. Вопишите и выберите подписку, используемую на странице [Подписки на портале Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Выберите **каталог Change.**
3. Просмотрите все предупреждения, которые отображаются, а затем выберите **Изменение**.
4. Каталог изменен для подписки, и вы получите сообщение об успехе.
5. Используйте *переключатель Directory,* чтобы перейти в новый каталог. Для правильного показа может потребоваться до 10 минут.

**Рекомендуемые документы**

- [Передача права собственности на подписку Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Перемещение ресурсов в новую группу ресурсов или подписку](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Управление ресурсами с помощью портала Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
