---
title: Правило отключенных подписок и учетных записей
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
- "9003559"
- "6676"
ms.openlocfilehash: 6a350c6bca18306e64f647cfa3a7f14fa204109b
ms.sourcegitcommit: 9626d39e5891f83774ba31574a00b0bae92ad442
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2020
ms.locfileid: "48755604"
---
# <a name="azure-subscription-disabled"></a>Подписка Azure отключена

Ваша подписка на Azure может быть отключена из-за истечения срока действия вашего кредита, истечения лимита расходов, выставления счета с истекшим сроком действия кредитных карт или из-за того, что Администратор учетной записи отменил подписку. Ниже приведены сведения о том, как можно повторно включить подписку. Дополнительные сведения: [Повторная активация подписки на Azure](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support)

**Повторное включение подписки на Azure (подписка была случайно отменена)** [Администратор учетной записи](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) может повторно активировать отмененную подписку "оплата от имени" в центре управления учетными записями:

1. Войдите в [центр учетных записей](https://account.windowsazure.com/Subscriptions).
2. Выберите отмененную подписку. Нажмите кнопку **Повторная активация**.

Для других типов подписки [обратитесь в службу поддержки](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade) , чтобы подписка была повторно активирована.

**Кредитная карта с истекшим сроком действия**

Когда вы подписываетесь на **бесплатную учетную запись Azure**, вы получаете бесплатную пробную подписку, которая предоставляет вам $200 в Azure в течение 30 дней и 12 месяцев бесплатного обслуживания. По истечении 30 дней Azure отключает подписку. Ваша Подписка отключена, чтобы защитить от постоянных затрат на использование за пределами кредитных и бесплатная службы, включенные в подписку. Для продолжения использования служб Azure необходимо [обновить подписку](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support). После обновления подписка по-прежнему имеет доступ к бесплатным службам в течение 12 месяцев. Вы получаете только оплату за использование за пределами бесплатной службы и количества.  
Дополнительные сведения: [просроченная кредитная карта](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support#your-credit-is-expired)

**Достигнут лимит расходов**

При достижении лимита расходов Azure отключает подписку на оставшуюся часть этого периода выставления счетов. Ваша Подписка отключена, чтобы защитить от постоянных расходов на использование за пределами кредита, включенного в подписку. Чтобы удалить лимит расходов, ознакомьтесь с [разделом лимиты расходов Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support).  
Дополнительные сведения: [достигнуто предельное число расходов](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled?WT.mc_id=Portal-Microsoft_Azure_Support#you-reached-your-spending-limit)

**Просроченный вексель**

Чтобы разрешить просроченное сальдо, ознакомьтесь [с разрешениями срока выполнения подписки на Azure после получения электронной почты из Azure](https://docs.microsoft.com/azure/billing/billing-azure-subscription-past-due-balance?WT.mc_id=Portal-Microsoft_Azure_Support).

**Счет превышает ограничение для кредитных карт**

Чтобы устранить эту проблему, [переключитесь на другую кредитную карту](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support). Если вы представляете предприятие, вы можете [переключиться на оплату по счету](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice?WT.mc_id=Portal-Microsoft_Azure_Support).

**Примечание**: новая дата юбилея подписки будет назначена повторно включенным подпискам. Количество дней (интервал), в течение которых подписка была приостановлена, будет добавлена к исходной дате СОПОСТАВЛЕНИЯ. Любая дата юбилея, которая припадает на 29, 30 или 31, приведет к тому, что Дата сопоставления безопасности устанавливается на первый из следующих месяцев.  
Пример:

- Первоначальный годовщина подписки 25-25;
- Подписка была приостановлена на 10/3 и повторно включена на 10/9;
- Подписка отключена в течение 6 дней (интервал 6);
- Затем этот интервал добавляется в исходное сопоставление безопасности, а сумма становится новой датой СОПОСТАВЛЕНИЯ (25 + 6 = 31). 

**Note**: в этом примере, так как Дата сопоставления безопасности теперь больше 28, Новая Дата сопоставления будет первой из следующих месяцев.

**Рекомендуемые документы**

- [Переключить подписку](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Отмена подписки](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/?source=datamarket)
- Обнаружение [администратора учетной записи](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- [Что делать, если моя подписка Azure становится недоступной?](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Лимит расходов Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
