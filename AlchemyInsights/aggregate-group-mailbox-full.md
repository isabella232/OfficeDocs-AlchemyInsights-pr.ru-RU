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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315923"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox полный NDR, полученный для электронной почты, отправленной Microsoft 365 группе

Используйте следующую команду EXO Shell для создания правила транспорта Exchange для бесшумного сброса электронных писем, отправленных в совокупный почтовый ящик группы:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Примечание.** Замените **SMTP-адрес в -SentTo** на SMTP-адрес совокупного группового почтового ящика в клиенте. Вы можете получить SMTP-адрес сводного группового почтового ящика из полученного NDR.



