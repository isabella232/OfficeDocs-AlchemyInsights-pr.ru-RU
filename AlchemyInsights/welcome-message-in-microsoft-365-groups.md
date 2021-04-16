---
title: Приветственное сообщение в группах Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: 6c46ba1b2c2c94e21d7c76e45df1d416ba423faf
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806419"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="4df12-102">Приветственное сообщение в группах Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4df12-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="4df12-103">Новые пользователи, присоединяющиеся к группе Microsoft 365, получат приветственное сообщение электронной почты, если для свойства "UnifiedGroupWelcomeMessageEnabled" установлено значение "Истина".</span><span class="sxs-lookup"><span data-stu-id="4df12-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="4df12-104">Если нужно отключить приветственное сообщение, используйте следующую команду [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="4df12-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
