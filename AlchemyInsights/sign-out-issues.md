---
title: Проблемы с выходом из учетной записи
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886899"
---
# <a name="sign-out-issues"></a>Проблемы с выходом из учетной записи

Чтобы устранить проблемы, связанные с выходом, выполните указанные ниже действия.

1. Если вы или пользователь выходите или исключаетесь из приложений, следуйте инструкциям в статьях [Настройка управления сеансом проверки подлинности с помощью условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) или [Настраиваемые жизненные циклы маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Большинство других ошибок и проблем с выходом можно решить, устраняя проблемы интеграции Azure Active Directory (Azure AD) с конкретным приложением. Рекомендации по конкретно интеграции можно найти в этом [наборе руководств, посвященных интеграции приложений в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), в том числе:
    - Руководства по приложению SaaS
    - Руководства по единому входу
    - Руководства по подготовке пользователей