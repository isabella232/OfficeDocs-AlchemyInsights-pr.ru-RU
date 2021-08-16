---
title: Передача прав владения на выставление счетов Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036109"
---
# <a name="transfer-azure-billing-ownership"></a>Передача прав владения на выставление счетов Azure

Войдите на [портал Azure](https://portal.azure.com/) в качестве администратора учетной записи для выставления счетов, содержащей подписку, которую вы хотите передать. Если вы не знаете, являетесь ли вы администратором или вам нужно определить, кто является администратором, см. раздел [Определение администратора выставления счетов для учетной записи](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Выполните поиск по запросу _Управление затратами + выставление счетов_.
1. Выберите **Подписки** в области слева. В зависимости от уровня доступа вам может потребоваться выбрать область выставления счетов, а затем нажать **Подписки** или **Подписки Azure**.
1. Выберите **Передать права владения на выставление счетов** для подписки, которую хотите передать.
1. Введите адрес электронной почты пользователя, являющегося администратором выставления счетов для учетной записи, которая станет новым владельцем подписки, а затем выберите **Отправить запрос на передачу**.
1. Пользователь получит сообщение электронной почты с инструкциями по проверке вашего запроса на передачу. Чтобы утвердить запрос на передачу, пользователь выбирает ссылку в сообщении электронной почты и следует инструкциям.

Обратите внимание, что если вы передаете права владения на выставление счетов учетной записи пользователя в другом клиенте Azure AD, все назначения по [управлению доступом на основе ролей (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для управления ресурсами в подписке безвозвратно удаляются. Доступ к управлению ресурсами в подписке будет иметь только новый владелец. Дополнительные сведения о способе изменения каталога для подписки см. в статье [Передача подписки пользователю в другом клиенте Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Важное воздействие на ваши счета**_: если вы передаете права владения на выставление счетов для подписки Azure, взимаемые суммы будут распределены пропорционально. Вы сможете получить доступ к счетам, следуя указанным ниже инструкциям.  

1. Выберите подписку на  [странице подписок](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) портала Azure [в качестве пользователя, имеющего доступ к счетам](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), затем нажмите  **Счета**.
1. Чтобы просмотреть копию счета в формате PDF, щелкните  **Скачать счет** . Если отображается  _Недоступно_, см. статью  [Почему не отображается счет за последний расчетный период?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. Просмотреть сведения о ежедневном использовании можно, щелкнув **расчетный период**, чтобы получить счет в формате PDF и копию подробного файла о ежедневном использовании (CSV-файл). Дополнительные сведения см. в разделе  [Сведения о счетах и данных об использовании](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Рекомендуемые документы**

- [Передача прав владения на выставление счетов подписки Azure в другую учетную запись](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Сведения о передаче прав владения на выставление счетов для подписки Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Передача подписок на разработку и тестирование с оплатой по мере использования в среде Visual Studio, Microsoft Partner Network (MPN)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Вопросы и ответы о передаче прав владения](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Устранение проблем при передаче прав владения](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
