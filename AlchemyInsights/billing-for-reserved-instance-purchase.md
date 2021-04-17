---
title: Выставление счета для покупки зарезервированного экземпляра
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820335"
---
# <a name="billing-for-reserved-instance-purchase"></a>Выставление счета для покупки зарезервированного экземпляра

Покупка зарезервированного экземпляра взимается с метода оплаты, привязанного к выбранной подписке на момент покупки. Тип подписки должен быть корпоративным соглашением (номер предложения: MS-AZR-0017P), Pay-As-You-Go (номер предложения: MS-AZR-0003P), Microsoft Customer Agreement или CSP.

- Для корпоративной подписки сборы вычитаются из денежного баланса обязательств по регистрации или взимаются в качестве переплаты.
- Для подписки Pay-As-You-Go плата взимается с кредитной карты или метода оплаты счета по подписке.

**Отмена резервирования**

- **Самообслуживка:** Вы можете самостоятельно отменить или обменять зарезервированный экземпляр с помощью [портала Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Выберите резервирование и нажмите кнопку возврата или обмена. Обратите внимание, что для обмена или возврата необходимо иметь доступ к владельцу в порядке бронирования. Доступ только к резервации не позволит вам приступить к возврату или обмену. Попросите владельца заказа бронирования предоставить владельцу доступ к заказу бронирования
- **Политика Exchange:** Вы можете обменять резервирование на другое бронирование того же типа — на обмене резервированием не предусмотрены **штрафные** санкции. Общая сумма обязательств с новым резервированием должна быть больше суммы возврата валютной резервации и будущих ежемесячных платежей (если применимо)
- **Политика возврата:** Сумма возврата и отмененные будущие платежи не могут превышать $50 000 USD в 12-месячном окне. В **настоящее время мы не взимаем** никаких штрафов за возврат, но можем взимать их с будущих возвратов.

**Исключения:** Возможности обмена и отмены самообслуживки недоступны для клиентов Соглашение Enterprise правительства США

- **Поддержка API/PS/CLI** недоступна для отмены и возврата средств для обмена самообслужива и возврата средств [для резервирования Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Возможности обмена и отмены самообслуживки недоступны для клиентов Соглашение Enterprise правительства США. Поддерживаются другие типы подписки правительства США, включая Pay-As-You-Go и CSP

Дополнительные данные. [Обработка](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) транзакций с возвратом и обменом Подробнее: Политики exchange [и Refund](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Другие вопросы: Посетите документы [зарезервированных экземпляров](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Обмен существующим зарезервированным экземпляром (Самообслуживка)**

Вы можете обменять резервирование на другое бронирование того же типа. Вы также можете вернуть резервирование, до $50 000 USD в год, если оно больше не требуется. Возможности обмена и отмены самообслуживки недоступны для клиентов Соглашение Enterprise правительства США. Поддерживаются другие типы подписки правительства США, включая Pay-As-You-Go и CSP. Для обмена или возврата существующего резервирования необходимо иметь доступ к владельцу в порядке бронирования.

Следующие действия будут направлять процедуру для завершения транзакции

1. Войдите на портал [Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Выберите резервирование, которое необходимо вернуть, и нажмите **кнопку Exchange** 2.Select продукт VM, который необходимо приобрести, и введите количество. Убедитесь, что общее количество новых покупок превышает сумму [возврата, определите правильный размер перед покупкой.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Обзор и завершение транзакции

**Возврат за зарезервированный экземпляр**

Чтобы вернуть резервирование, перейдите к **сведениям о резервировании** и нажмите кнопку **Возврат**

**Pro-rated refund:**

**Примеры pro-ration и минимальных требований для возврата и обмена** Пример предварительного резервирования:

- С 1 января вы приобретаете однолетний ri сроком на $120.
- 7 апреля вы хотите вернуть или обменять это бронирование
- Так как бронирование было в живых в течение 97 дней, вы получите (1-97/365) * $ 120 назад. (например, $88.1). В настоящее время нет штрафа за возврат средств
- При обмене новая покупка должна быть больше $88.1
- В настоящее время не существует штрафа за возврат средств

**Пример резервирования плана биллинга:**

- Вы покупаете однолетний срок ri за $10 в месяц
- 7 апреля вы хотите вернуть или обменять это бронирование
- Так как последний платеж был 7 дней, вы получите (1-7/31) * $ 10 назад. (например, $7,74)
- Будущие отмененные платежи — $80. В настоящее время нет штрафа за возврат средств
- Эта отмена будет вычитать $87.74 из лимита возврата $50,000
- При обмене общее значение новой покупки должно быть больше $ 87,74

**Невозможно увидеть счет за последний период выставления счетов**

Возможные причины, по которой может не быть выставлен счет:

- У вас есть ежемесячная кредитная сумма с подпиской, которая не превышала или у вас есть бесплатная пробная версия. Счет создается только в том случае, если вы задолжали деньги
- Это менее 30 дней со дня подписки на Azure
- Счет еще не создан. Подождите, пока не закончится период вы выставления счета
- Если вы не администратор учетной записи, старые счета могут быть недоступны для вас

**Скачайте счет с портала Azure (.pdf)**

- Выберите подписку со страницы [Подписки](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) на портале Azure в качестве пользователя с [доступом к счетам](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Выбор **счетов**
- Чтобы просмотреть копию счета в формате PDF, щелкните **Скачать счет**. Если отображается **Недоступно**, см. статью [Почему не отображается счет за последний расчетный период?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Получение счета по электронной почте (.pdf)**

- Выберите подписку со страницы [Подписки.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Щелкните **Счета-фактуры,** а затем отправьте мой счет по электронной почте
- Щелкните **выбрать и** принять условия. Вам придется выбрать для каждой подписки у вас есть

Примечание. Если вы не получите сообщение электронной почты после следующих действий, убедитесь, что ваш адрес электронной почты является правильным в предпочтениях связи [в профиле](https://account.windowsazure.com/profile)

**Скачайте данные об использовании с портала Azure**

- Вход в [Центр учетных записей Azure](https://account.windowsazure.com/Subscriptions) в качестве [администратора учетной записи](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Выберите подписку, для которой нужны сведения о счете и использовании
- Выбор **истории биллинга**
- Выберите **представление текущего заявления,** чтобы просмотреть оценку ваших сборов на момент сгенерирования оценки
- Выберите **использование загрузки** для загрузки данных об использовании в качестве CSV-файла. Если доступны две версии, скачайте версию 2

Другие вопросы: [Посетите документы зарезервированных экземпляров](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Рекомендуемые документы**

- [Основы биллинга](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Понимание того, как применяется скидка Reserved Instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Загрузка или просмотр счетов-фактур Azure и данных об использовании в день](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Понимание того, как применяется скидка Reserved Instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Понимание использования зарезервированных экземпляров для подписки Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Понимание использования зарезервированных экземпляров для регистрации предприятия](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Расходы на программное обеспечение Для Windows, не включенные в зарезервированные экземпляры](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserved Instances in Partner Central Cloud Solution Provider (CSP) program](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)