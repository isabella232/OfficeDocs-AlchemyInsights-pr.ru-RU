---
title: Восстановление удаленной группы Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505701"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Восстановление удаленной группы Microsoft 365

Вы можете восстановить удаленную группу Microsoft 365 или Microsoft Teams в течение 30 дней после удаления.

1. Чтобы войти в центр администрирования Microsoft 365 и перечислить удаленные группы и группы, перейдите в центр администрирования [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)

    **Примечание:** Войдите в систему с помощью учетной записи, назначенной администратору клиента или роли администратора групп.

1. Выберите удаленную группу Microsoft 365/Teams, которая будет восстановлена, и щелкните **группу восстановления.**

    Если группа не может быть восстановлена из-за конфликтующих smTP-адресов, используйте следующую команду, чтобы найти объект, вызывающий конфликт, и удалить адрес SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Примечание:** В некоторых случаях для восстановления группы и всех ее данных может потребоваться до 24 часов.

    Дополнительные сведения или сведения о восстановлении групп с помощью PowerShell см. в руб. Восстановление удаленных групп [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)