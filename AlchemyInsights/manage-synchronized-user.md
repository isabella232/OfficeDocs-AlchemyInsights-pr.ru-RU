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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380518"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Не удается задать основной адрес электронной почты или изменить атрибуты пользователя

Если для вашей среды включена синхронизация службы каталогов, некоторые атрибуты пользователя или объекта невозможно изменить с помощью центра администрирования.
Чтобы полностью управлять синхронизированными пользователями и всеми их атрибутами, используйте локальную консоль управления пользователями и группами Active Directory (adsiedit. msc).  

Кроме того, вы можете изменить отдельных пользователей или атрибуты для синхронизированных пользователей с помощью PowerShell, как показано в следующих примерах: 
- Set – MsolUser — UserPrincipalName user@yourdomain.onmicrosoft.com — Алтернатимаиладдрессес user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"
- Remove — MsolUser — UserPrincipalName "user@yourdomain.onmicrosoft.com