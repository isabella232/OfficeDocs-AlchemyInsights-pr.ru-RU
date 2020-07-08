---
title: Сообщения, отправленные в группу Microsoft 365, не получены всеми участниками
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2020
ms.locfileid: "45047241"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Сообщения, отправленные в группу Microsoft 365, не получены всеми участниками

Убедитесь в том, что все участники группы подписаны на получение сообщений. См. статью [Присоединение к группе в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Чтобы проверить состояние сообщений участников, которые подписались на групповые сообщения электронной почты, выполните следующую команду на странице [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`