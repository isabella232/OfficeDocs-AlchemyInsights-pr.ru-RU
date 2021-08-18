---
title: Управление синхронизированным пользователем
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114791"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Невозможно установить основной адрес электронной почты, изменить атрибуты пользователей или удалить или удалить синхронизированного пользователя

Если для среды включена синхронизация каталогов, некоторые атрибуты пользователя или объекта нельзя изменить с помощью Центр администрирования Microsoft 365.

Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальные активные пользователи каталогов и консоль управления группами (adsiedit.msc).  

Кроме того, можно изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью powershell, как показано в этих распространенных примерах:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
