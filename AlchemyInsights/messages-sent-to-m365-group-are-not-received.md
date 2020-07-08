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
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="e2a16-102">Сообщения, отправленные в группу Microsoft 365, не получены всеми участниками</span><span class="sxs-lookup"><span data-stu-id="e2a16-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="e2a16-103">Убедитесь в том, что все участники группы подписаны на получение сообщений.</span><span class="sxs-lookup"><span data-stu-id="e2a16-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="e2a16-104">См. статью [Присоединение к группе в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="e2a16-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="e2a16-105">Чтобы проверить состояние сообщений участников, которые подписались на групповые сообщения электронной почты, выполните следующую команду на странице [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="e2a16-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`