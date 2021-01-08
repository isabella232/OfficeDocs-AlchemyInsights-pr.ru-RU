---
title: Изменение адреса электронной почты группы Microsoft 365 или Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756570"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Изменение адреса электронной почты группы Microsoft 365 или Microsoft Teams

Вы можете изменить адрес электронной почты группы Microsoft 365 или Microsoft Teams с помощью [Центра администрирования Microsoft 365](https://admin.microsoft.com/). Достаточно выбрать группу, а затем выбрать @Изменить адрес электронной почты.

Также можно использовать следующую команду EXO PowerShell, чтобы изменить основной SMTP-адрес группы Microsoft 365 или Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Пример:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
