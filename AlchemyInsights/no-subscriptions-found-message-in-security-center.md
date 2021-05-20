---
title: В центре безопасности получено сообщение о том, что подписки не найдены
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544121"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>В центре безопасности получено сообщение о том, что подписки не найдены

При доступе к Центру безопасности в Microsoft Defender появляется сообщение "Подписки не найдены". Это означает, что служба Azure Active Directory (AAD), используемая для входа пользователя на портал, не имеет лицензии на ATP в Microsoft Defender.  

Лицензии Windows E5 и Office E5 — это две отдельные лицензии.

Если лицензия была приобретена, но не подготовлена для данного экземпляра AAD, создайте запрос в службу поддержки. Возможные варианты: <br/>
-   Возможная проблема при предоставлении лицензии.<br/>
-   По ошибке лицензия была предоставлена другому экземпляру Microsoft AAD, а не тому, который используется для проверки подлинности в службе.