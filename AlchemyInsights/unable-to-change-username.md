---
title: Не удалось изменить имя пользователя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798677"
---
# <a name="unable-to-change-username"></a>Не удалось изменить имя пользователя

В некоторых случаях изменения UPN (UserPrincipalName) не распространяются на облако. Вы можете столкнуться с ошибками проверки на портале Office 365 или с невозможностью изменить имя пользователя или адрес электронной почты. Чтобы устранить эту проблему, вручную настройте UserPrincipalName с помощью этой команды PowerShell.

**Пример: переименование пользователя**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Эта команда переименовывает davidc@contoso.com в davidchew@contoso.com.

Дополнительные сведения см. в статье [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).