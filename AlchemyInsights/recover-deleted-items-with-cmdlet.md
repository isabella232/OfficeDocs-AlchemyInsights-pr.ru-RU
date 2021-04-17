---
title: Восстановление удаленных элементов с помощью командлета
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835824"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="ac8fe-102">Восстановление удаленных элементов с помощью командлета</span><span class="sxs-lookup"><span data-stu-id="ac8fe-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="ac8fe-103">Используйте командлет [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) для просмотра удаленных элементов в почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="ac8fe-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="ac8fe-104">Для восстановления удаленных элементов используйте командлет [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ac8fe-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="ac8fe-105">Подробные сведения см. в статье [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ac8fe-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="ac8fe-106">Перед выполнением этого командлета вам должна быть назначена роль "Импорт и экспорт почтовых ящиков".</span><span class="sxs-lookup"><span data-stu-id="ac8fe-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="ac8fe-107">Дополнительные сведения см. в статье [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ac8fe-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
