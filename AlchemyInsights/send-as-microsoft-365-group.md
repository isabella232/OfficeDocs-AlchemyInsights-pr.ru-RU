---
title: Отправить как группе Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46853013"
---
# <a name="send-as-microsoft-365-group"></a>Отправить как группе Microsoft 365

Чтобы разрешить определенным пользователям отправлять сообщения как группе Microsoft 365, можно назначить разрешения "Отправить как".  

1. Подключитесь к Exchange Online PowerShell.  

2. Выполните следующую команду:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Дополнительные сведения см. в статье [Предоставление участникам разрешений "Отправить как" или "Отправить от имени группы"](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).