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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="929c9-102">Отправитель не получает письма, отправленные в группу Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="929c9-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="929c9-103">По умолчанию отправитель сообщения электронной почты в группу Microsoft 365 не получает копию сообщения в свою папку "Входящие", даже если отправитель является участником группы.</span><span class="sxs-lookup"><span data-stu-id="929c9-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="929c9-104">Используйте эту команду PowerShell EXO, чтобы разрешить отправителю получать копию каждого письма, отправляемого в группу Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="929c9-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="929c9-105">Чтобы включить параметр для всех почтовых ящиков одновременно:</span><span class="sxs-lookup"><span data-stu-id="929c9-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="929c9-106">**Примечание**. Вступление изменений этого параметра в силу занимает до часа.</span><span class="sxs-lookup"><span data-stu-id="929c9-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>