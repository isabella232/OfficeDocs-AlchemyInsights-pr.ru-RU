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
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="c4fd8-102">Приветственное сообщение в группах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c4fd8-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="c4fd8-103">Новые пользователи, присоединяющиеся к группе Microsoft 365, получат приветственное сообщение электронной почты, если для свойства "UnifiedGroupWelcomeMessageEnabled" установлено значение "Истина".</span><span class="sxs-lookup"><span data-stu-id="c4fd8-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="c4fd8-104">Если нужно отключить приветственное сообщение, используйте следующую команду [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="c4fd8-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
