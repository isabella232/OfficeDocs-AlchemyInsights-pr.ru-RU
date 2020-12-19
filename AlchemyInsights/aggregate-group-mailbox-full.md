---
title: Полный NDR AggregateGroupMailbox, полученный для электронной почты, отправленной в группу Microsoft 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715727"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="91ea2-102">Полный NDR AggregateGroupMailbox, полученный для электронной почты, отправленной в группу Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="91ea2-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="91ea2-103">Используйте следующую команду EXO Shell, чтобы создать правило транспорта Exchange для отправки сообщений электронной почты в почтовый ящик группы в тихом режиме:</span><span class="sxs-lookup"><span data-stu-id="91ea2-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="91ea2-104">Замените SMTP-адрес в **-SentTo** SMTP-адресом сводного почтового ящика группы в клиенте.</span><span class="sxs-lookup"><span data-stu-id="91ea2-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="91ea2-105">SmTP-адрес сводного почтового ящика группы можно получить из полученного сообщения о NDR.</span><span class="sxs-lookup"><span data-stu-id="91ea2-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



