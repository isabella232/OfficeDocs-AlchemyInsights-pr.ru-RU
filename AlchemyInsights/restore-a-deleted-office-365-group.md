---
title: Восстановление удаленной Microsoft 365 группы
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959039"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Восстановление удаленной Microsoft 365 группы

Вы можете восстановить удаленную группу Microsoft 365 или Microsoft Teams в течение 30 дней после удаления.

1. Перейдите [в Центр администрирования Microsoft 365,](https://aka.ms/RestoreDeletedGroup) чтобы войти в список удаленных групп и групп.

    **Примечание:** Войдите в систему с помощью учетной записи, назначенной администратору клиента или роли администратора групп.

1. Выберите удаленную группу Microsoft 365/Teams, которая будет восстановлена, и щелкните **группу восстановления.**

    Если группа не может быть восстановлена из-за конфликтующих smTP-адресов, используйте следующую команду, чтобы найти объект, вызывающий конфликт, и удалить адрес SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Примечание:** В некоторых случаях для восстановления группы и всех ее данных может потребоваться до 24 часов.

    Дополнительные сведения или сведения о восстановлении групп с помощью PowerShell см. в этой Microsoft 365 [группы.](https://go.microsoft.com/fwlink/?linkid=867802)