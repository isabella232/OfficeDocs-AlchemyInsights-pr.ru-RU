---
title: Разрешения календаря
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819921"
---
# <a name="calendar-permissions"></a>Разрешения календаря

Пользователи могут изменять свои собственные разрешения календаря с Outlook в Интернете или других клиентах, но в качестве администратора вам может потребоваться также исследовать.  
С помощью cmdlet Exchange PowerShell вы сможете получить разрешение в календаре пользователя:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Дополнительные сведения см. в следующих сведениях:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Разрешения календаря используются в совместном использовании календарей, чтобы узнать больше о совместном использовании календаря Outlook, см. в статьях:

- [Предоставление общего доступа к календарю Outlook другим пользователям](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Поделитесь календарем в Outlook в Интернете для бизнеса](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Для устранения неполадок в Calendar Permission можно использовать средство помощника по поддержке и [восстановлению.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)