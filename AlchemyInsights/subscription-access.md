---
title: Доступ к подписке
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773781"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Не удается выполнить вход в Azure из-за проблем с браузером (зависание браузера, не загружается, не загружается и т. д.).

Возможно, вы повлияли на отключение. Проверьте, существует ли непрерывный сбой: [состояние работоспособности Azure](https://status.azure.com/status/history/).

Выйдите из всех активных сеансов Azure. Запустите собственный или инкогнито режим веб-браузера.

Вы также можете попробовать обновить браузер, использовать другой браузер, удалить файлы cookie кэша, если они не работают.

Дополнительные сведения: [Устранение проблем с входом](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Не удается получить доступ к подпискам**

На [портале Azure](https://portal.azure.com/)убедитесь, что выбран правильный каталог Azure из учетной записи в правом верхнем углу.

В [центре учетных записей Azure](https://account.windowsazure.com/Subscriptions)убедитесь, что используемая учетная запись является администратором учетной записи.

Дополнительные сведения: [Устранение неполадок подписки не найдены](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Не удается получить доступ к журналу выставления счетов**

Администратору учетной записи необходимо убедиться, что пользователь, обращающийся к сведениям для выставления счетов, добавлен в Azure Active Directory в качестве пользователя-гостя: [Добавление или удаление нового пользователя](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Затем пользователю должна быть назначена роль глобального администратора: [назначение роли пользователям](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Опубликовать это, пользователю может быть предоставлен доступ к оплате с помощью политик RBAC: [предоставление доступа к выставлению счетов](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Рекомендуемые документы**

-   [Не удается выполнить вход для управления моей подпиской Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)