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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999253"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Не удается войти в Azure из-за проблем с браузером (браузер зависает, продолжает вращаться, не загружается и т.д.)

На вас может повлиять отключение. Проверьте, не существует ли сохраняющееся отключение: [Состояние здоровья Azure.](https://status.azure.com/status/history/)

Войдите во все активные сеансы Azure. Запустите закрытый или инкогнито-режим веб-браузера.

Вы также можете попробовать обновить браузер, использовать другой браузер, удалить файлы cookie кэша, если выше не работает.

Дополнительные новости. [Проблемы с входом в окантовку устранения неполадок](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Невозможно получить доступ к подпискам**

На [портале Azure](https://portal.azure.com/)убедитесь, что правильный каталог Azure выбран из учетной записи в правом верхнем справа.

В центре [учетной записи Azure](https://account.windowsazure.com/Subscriptions)убедитесь, что используемая учетная запись является администратором учетной записи.

Дополнительные новости. [Устранение неполадок, не найденных подписок](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Невозможно получить доступ к истории биллинга**

Администратор учетной записи должен убедиться, что пользователь, который получает доступ к сведениям о выставлении счетов, добавляется в каталог Azure Active в качестве гостевого пользователя: Добавьте или удалите [нового пользователя.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Затем пользователю должна быть предоставлена роль глобального администратора: [назначение роли пользователям.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

После этого пользователю может быть предоставлен доступ к выставлению счета с помощью политик RBAC: [Предоставление доступа к выставлению счета.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Рекомендуемые документы**

-   [Я не могу войти, чтобы управлять подпиской Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)