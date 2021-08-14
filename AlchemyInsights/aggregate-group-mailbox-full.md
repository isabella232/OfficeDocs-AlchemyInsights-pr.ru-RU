---
title: AggregateGroupMailbox полный NDR, полученный для электронной почты, отправленной Microsoft 365 группе
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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951866"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox полный NDR, полученный для электронной почты, отправленной Microsoft 365 группе

Используйте следующую команду EXO Shell для создания правила транспорта Exchange для бесшумного сброса электронных писем, отправленных в совокупный почтовый ящик группы:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Замените **smTP-адрес в -SentTo** на SMTP-адрес совокупного почтового ящика группы в клиенте. Вы можете получить SMTP-адрес сводного группового почтового ящика из полученного NDR.



