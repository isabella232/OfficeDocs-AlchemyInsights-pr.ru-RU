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
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020241"
---
# <a name="unable-to-change-username"></a>Не удалось изменить имя пользователя

В некоторых случаях изменения UPN (UserPrincipalName) не распространяются на облако. Вы можете столкнуться с ошибками проверки на портале Office 365 или с невозможностью изменить имя пользователя или адрес электронной почты. Чтобы устранить эту проблему, вручную настройте UserPrincipalName с помощью этой команды PowerShell.

**Пример: переименование пользователя**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Эта команда переименовывает davidc@contoso.com в davidchew@contoso.com.

Дополнительные сведения см. в статье [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).