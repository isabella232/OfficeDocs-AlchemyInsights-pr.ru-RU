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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768528"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>В центре безопасности получено сообщение о том, что подписки не найдены

При доступе к центру безопасности Microsoft Defender появляется сообщение "не найдено подписок". Это означает, что служба Azure Active Directory (AAD), используемая для входа пользователя на портал, не имеет лицензии на Microsoft Defender ATP.  

Лицензии Windows E5 и Office E5 - это две разные лицензии.

Если лицензия была приобретена, но не выделена для данного экземпляра AAD, откройте обращение в службу поддержки. Возможные варианты: <br/>
-   Возможная проблема при предоставлении лицензии.<br/>
-   По ошибке лицензия была предоставлена другому экземпляру Microsoft AAD, а не тому, который используется для проверки подлинности в службе.