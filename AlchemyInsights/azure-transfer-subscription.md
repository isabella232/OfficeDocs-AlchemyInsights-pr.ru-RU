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
# <a name="transfer-azure-billing-ownership"></a>Передача прав владения на выставление счетов Azure

Войдите на [портал Azure](https://portal.azure.com/) в качестве администратора учетной записи по выставлению счетов, содержащей подписку, которую вы хотите передать. Если вы не знаете, являетесь ли вы администратором или вам нужно определить, кто является администратором, см. раздел [Определение администратора выставления счетов для учетной записи](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Выполните поиск по запросу **Управление затратами + выставление счетов**.
- Выберите **Подписки** в области слева. В зависимости от уровня доступа вам может потребоваться выбрать область выставления счетов, а затем нажать **Подписки** или **Подписки Azure**.
- Выберите **Передать права владения на выставление счетов** для подписки, которую хотите передать.
- Введите адрес электронной почты пользователя, который является администратором выставления счетов для учетной записи, которая станет новым владельцем подписки, а затем выберите пункт **Отправить запрос на передачу**
- Пользователь получит сообщение электронной почты с инструкциями по проверке вашего запроса на передачу. Чтобы утвердить запрос на передачу, пользователь выбирает ссылку в сообщении электронной почты и следует инструкциям.

**Примечание**. Если вы передаете права владения на выставление счетов учетной записи пользователя в другом клиенте Azure AD, все назначения по [управлению доступом на основе ролей (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для управления ресурсами в подписке безвозвратно удаляются. Доступ к управлению ресурсами в подписке будет иметь только новый владелец. Дополнительные сведения см. в статье [Передача подписки пользователю в другом клиенте Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Рекомендуемые документы**

- [Передача прав владения на выставление счетов подписки Azure в другую учетную запись](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Сведения о передаче прав владения на выставление счетов для подписки Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Передача подписок на разработку и тестирование с оплатой по мере использования в среде Visual Studio, Microsoft Partner Network (MPN)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Вопросы и ответы о передаче прав владения](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Устранение проблем при передаче прав владения](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
