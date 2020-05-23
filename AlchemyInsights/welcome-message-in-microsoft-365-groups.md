---
title: Приветственное сообщение в группах Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44320475"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Приветственное сообщение в группах Microsoft 365

Новые пользователи, присоединяющиеся к группе Microsoft 365, получат приветственное сообщение электронной почты, если для свойства "UnifiedGroupWelcomeMessageEnabled" установлено значение "Истина".

Если нужно отключить приветственное сообщение, используйте следующую команду [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps):

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
