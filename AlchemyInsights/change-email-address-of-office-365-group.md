---
title: Изменение адреса электронной почты группы Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282469"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Изменение адреса электронной почты группы Microsoft 365

Можно изменить адрес электронной почты группы Microsoft 365, используя центр администрирования. Достаточно выбрать группу, а затем выбрать @Изменить адрес электронной почты.

Также можно использовать следующую команду EXO PowerShell, чтобы изменить основной SMTP-адрес группы Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Пример:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
