---
title: Сообщения, отправленные в группу Microsoft 365, не получены всеми участниками
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480696"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Сообщения, отправленные в группу Microsoft 365, не получены всеми участниками

Убедитесь в том, что все участники группы подписаны на получение сообщений. См. статью [Присоединение к группе в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Чтобы проверить состояние сообщений участников, которые подписались на групповые сообщения электронной почты, выполните следующую команду на странице [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Используйте следующую команду EXO PowerShell, чтобы настроить для всех участников группы доставку в их почтовые ящики сообщений электронной почты, отправленных в группу Microsoft 365:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Пример:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`