---
title: Не удается получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959507"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не удается подключиться к общедоступным папкам

Если доступ к общедоступным папкам не работает для нескольких пользователей, выполните указанные ниже действия.

Подключитесь к EXO PowerShell и настройте DefaultPublicFolderMailbox учетной записи пользователя, чтобы она соотнесена с одной учетной записью пользователя.

Пример:

Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс

Set – Mailbox Проблемусер — значение \<DefaultPublicFolderMailbox из предыдущей команды>

Чтобы изменения вступили в силу, подождите хотя бы один час.