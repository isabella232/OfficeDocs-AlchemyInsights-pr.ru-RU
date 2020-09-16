---
title: Отправитель не получает письма, отправленные в группу Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751328"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Отправитель не получает письма, отправленные в группу Microsoft 365

По умолчанию отправитель сообщения электронной почты в группу Microsoft 365 не получает копию сообщения в свою папку "Входящие", даже если отправитель является участником группы.

Используйте эту команду PowerShell EXO, чтобы разрешить отправителю получать копию каждого письма, отправляемого в группу Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Чтобы включить параметр для всех почтовых ящиков одновременно:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Примечание**. Вступление изменений этого параметра в силу занимает до часа.