---
title: Отправитель не получает письма, отправленные в группу Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46846061"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Отправитель не получает письма, отправленные в группу Microsoft 365

По умолчанию отправитель сообщения электронной почты в группу Microsoft 365 не получает копию сообщения в свою папку "Входящие", даже если отправитель является участником группы.

Используйте эту команду PowerShell EXO, чтобы разрешить отправителю получать копию каждого письма, отправляемого в группу Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Чтобы включить параметр для всех почтовых ящиков одновременно:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Примечание**. Вступление изменений этого параметра в силу занимает до часа.