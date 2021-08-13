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
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958310"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Отправитель не получает письма, отправленные в группу Microsoft 365

По умолчанию отправитель сообщения электронной почты в группу Microsoft 365 не получает копию сообщения в свою папку "Входящие", даже если отправитель является участником группы.

Используйте эту команду PowerShell EXO, чтобы разрешить отправителю получать копию каждого письма, отправляемого в группу Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Чтобы включить параметр для всех почтовых ящиков одновременно:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Примечание**. Вступление изменений этого параметра в силу занимает до часа.