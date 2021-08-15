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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993906"
---
# <a name="delete-tenant"></a>Удаление клиента

Чтобы удалить Azure AD, убедитесь, что:
- Вы глобальный администратор в каталоге.
- Вы не подписаны с учетной записью, которая имеет каталог по умолчанию, например contoso.onmicrosoft.com в подписанной учетной записи, например admin@contoso.onmicrosoft.com.
- Удалите все активные приложения в каталоге перед удалением. Чтобы удалить активные приложения, перейдите к регистрациям приложений и удалите существующие приложения.
- В каталоге не существует активных Microsoft Online Services, например Microsoft Azure, Office 365 или Azure AD Premium, связанных с каталогом. Перенос подписки или ускорение отмены активных подписок с помощью службы поддержки Azure и биллинга. Дополнительные новости о том, как отменить подписки Office 365 Azure. Инструкции по связыванию или добавлению существующей подписки на клиента см. в журнале Associate или добавить подписку Azure в клиент [Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Нет лицензии Active. Чтобы удалить лицензии, см. [в журнале How to remove Subscription to Remove license.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- В каталоге нет других активных пользователей, кроме вас, как глобального администратора при попытке удалить Azure AD. Удалите других активных пользователей, а также необходимо удалить все зависимости от настраиваемого доменного имени клиента, например пользователей, созданных с admin@contoso.com.

Дополнительные действия по:
- Удаление "Azure Active Directory" или "подписка", см. [в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Удаление приложений в каталоге см. в руб. [Удаление приложений.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
