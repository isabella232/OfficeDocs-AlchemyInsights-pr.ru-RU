---
title: Не удалось изменить имя пользователя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431742"
---
# <a name="unable-to-change-username"></a>Не удалось изменить имя пользователя

В некоторых случаях изменения UPN (UserPrincipalName) не распространяются на облако. Вы можете столкнуться с ошибками проверки на портале Office 365 или с невозможностью изменить имя пользователя или адрес электронной почты. Чтобы устранить эту проблему, вручную настройте UserPrincipalName с помощью этой команды PowerShell.

**Пример: переименование пользователя**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Эта команда переименовывает davidc@contoso.com в davidchew@contoso.com.

Дополнительные сведения см. в статье [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).