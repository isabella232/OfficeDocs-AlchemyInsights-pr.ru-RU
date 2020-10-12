---
title: Изменение адреса электронной почты группы Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416702"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Изменение адреса электронной почты группы Microsoft 365

Вы можете изменить адрес электронной почты группы Microsoft 365, используя Центр администрирования. Достаточно выбрать группу, а затем выбрать @Изменить адрес электронной почты.

Также можно использовать следующую команду EXO PowerShell, чтобы изменить основной SMTP-адрес группы Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Пример:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
