---
title: Изменение адреса электронной почты группы Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930742"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Изменение адреса электронной почты группы Microsoft 365

Вы можете изменить адрес электронной почты группы Microsoft 365, используя Центр администрирования. Достаточно выбрать группу, а затем выбрать @Изменить адрес электронной почты.

Также можно использовать следующую команду EXO PowerShell, чтобы изменить основной SMTP-адрес группы Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Пример:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
