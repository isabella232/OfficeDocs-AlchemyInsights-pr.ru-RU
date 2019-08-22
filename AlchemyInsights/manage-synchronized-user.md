---
title: Управление синхронизированным пользователем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542015"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Не удается задать основной адрес электронной почты или изменить атрибуты пользователя

Если для вашей среды включена синхронизация службы каталогов, некоторые атрибуты пользователя или объекта невозможно изменить с помощью центра администрирования Microsoft 365.

Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальную консоль управления пользователями и группами Active Directory (adsiedit. msc).  

Кроме того, вы можете изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью PowerShell, как показано в следующих примерах: 
- Set – MsolUser — UserPrincipalName user@yourdomain.onmicrosoft.com — Алтернатимаиладдрессес user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"
- Remove — MsolUser — UserPrincipalName "user@yourdomain.onmicrosoft.com