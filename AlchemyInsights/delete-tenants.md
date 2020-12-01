---
title: Удаление клиента
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477705"
---
# <a name="delete-tenant"></a>Удаление клиента

Чтобы удалить Azure AD, убедитесь, что:
- Вы являетесь глобальным администратором каталога.
- Вы не вошли в систему с помощью учетной записи, имеющей каталог по умолчанию, например contoso.onmicrosoft.com, в учетной записи с входом в систему, например admin@contoso.onmicrosoft.com.
- Перед удалением удалите все активные приложения в каталоге. Чтобы удалить активные приложения, перейдите к разделу Регистрация приложений и удалите существующие приложения.
- Нет активных подписок для всех служб Microsoft Online, таких как Microsoft Azure, Office 365 или Azure AD Premium, связанных с каталогом. Перенесите свои подписки или упростите отмену активных подписок с помощью поддержки и выставления счетов в Azure. Узнайте больше о том, как отказаться от использования подписок на Office 365 и Azure. Рекомендации по связыванию или добавлению существующей подписки на клиент можно узнать в статье [связывание или Добавление подписки Azure к клиенту Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Отсутствует активная лицензия. Чтобы удалить лицензии, ознакомьтесь со статьей [Удаление подписки для удаления лицензии](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- В каталоге нет других активных пользователей, кроме глобального администратора при попытке удалить Azure AD. Удалите все остальные активные пользователи, Кроме того, необходимо удалить все зависимости от имени пользовательского домена в клиенте, например пользователей, созданных с помощью admin@contoso.com.

Для получения более подробных инструкций:
- Delete "Azure Active Directory" или "Subscription", ознакомьтесь со статьей [Удаление Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Удалению приложений в каталоге можно узнать в статье [Удаление приложений](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
