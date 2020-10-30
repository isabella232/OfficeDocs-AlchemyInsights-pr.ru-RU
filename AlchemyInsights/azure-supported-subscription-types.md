---
title: Поддерживаемые типы подписки
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791478"
---
# <a name="supported-subscription-types"></a>Поддерживаемые типы подписки

Для продолжения ознакомьтесь с информацией о поддерживаемых типах подписки.

[Поддерживаемые типы подписки](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Передача прав владения на выставление счетов**

Портал Azure в качестве [Администратора учетной записи](https://ms.portal.azure.com/) для учетной записи по выставлению счетов, содержащей подписку, которую вы хотите передать.

- Найдите **Управление затратами и выставление счетов** Выберите **Подписки** в области слева. В зависимости от доступа может потребоваться выбрать область выставления счетов, а затем выбрать **Подписки** или **Подписки Azure** .
- Выберите "Передать права владения на выставление счетов" для подписки, которую хотите передать
- Введите адрес электронной почты пользователя, который является администратором выставления счетов для учетной записи, которая станет новым владельцем подписки, а затем выберите пункт **Отправить запрос на передачу**
- Пользователь получит сообщение электронной почты с инструкциями по проверке вашего запроса на передачу. Чтобы утвердить запрос на передачу, пользователь выбирает ссылку в сообщении электронной почты и следует инструкциям.

Примечание: если вы передаете права владения на выставление счетов учетной записи пользователя в другом клиенте Azure AD, то все задания по [управлению доступом на основе ролей (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для управления ресурсами в подписке безвозвратно удаляются. Доступ к управлению ресурсами в подписке будет иметь только новый владелец. Дополнительные сведения см. в статье [Передача подписки пользователю в другом клиенте Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Передача прав владения подпиской**

Для управления ресурсами подписки передача прав владения подпиской предварительно требует наличия доступа на основе ролей (RBAC), однако доступ к ним теряется. Дополнительные сведения о добавлении существующей подписки к клиенту см. в статье [Связать или добавить подписку Azure к Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Подписка с уже имеющейся непогашенной суммой по текущему циклу выставления счетов не будет передана в новый инструмент оплаты в новой учетной записи. У пользователей с новой учетной записью будет доступ только к сведениям о затратах за последний месяц по вашей подписке. Остальные журналы использования и выставления счетов не будут переданы вместе с подпиской.
- Передача прав владения на выставление счетов в рамках Соглашения Enterprise (EA) в настоящее время поддерживается только на портале Соглашения Enterprise
- При передаче подписки, ориентированной на кредитование, например Visual Studio, BizSpark, Microsoft Partner Network, новому пользователю требуется наличие лицензии Visual Studio/Microsoft partner network, чтобы принять запрос на передачу
- Все ресурсы, такие как виртуальные машины, диски и веб-сайты, успешно передаются в новую учетную запись. При передаче подписки между клиентами могут быть затронуты некоторые ресурсы:

**Доменные службы Azure AD**

Azure Key Vaults

- Могут быть затронуты [пользователи и базы данных, связанные с SQL,](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) особенно если клиент использует проверку подлинности, связанную с Azure Active Directory.
- Это может повлиять на работу **служб приложений** , для которых настроена проверка подлинности с помощью Azure Active Directory
- Учетные записи служб **Visual Studio Team** , подключенные к подпискам Azure, могут временно потерять доступ при отмене подписки, подключенной к Azure

**Рекомендуемые документы**

Шаги после принятия прав владения на выставление счетов:

- Чтобы сохранить права владения на выставление счетов, а также изменить тип подписки, см. статью [Переключение подписки Azure на другое предложение](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Передача подписок на разработку и тестирование с оплатой по мере использования в среде Visual Studio, Microsoft Partner Network (MPN)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Передача подписок с правами владения на выставление счетов для Соглашения Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Вопросы и ответы о передаче прав владения](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Устранение проблем при передаче прав владения](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)