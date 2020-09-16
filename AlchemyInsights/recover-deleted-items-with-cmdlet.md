---
title: Восстановление удаленных элементов с помощью командлета
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741316"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="16eb0-102">Восстановление удаленных элементов с помощью командлета</span><span class="sxs-lookup"><span data-stu-id="16eb0-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="16eb0-103">Используйте командлет [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) для просмотра удаленных элементов в почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="16eb0-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="16eb0-104">Для восстановления удаленных элементов используйте командлет [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="16eb0-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="16eb0-105">Подробные сведения см. в статье [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="16eb0-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="16eb0-106">Перед выполнением этого командлета вам должна быть назначена роль "Импорт и экспорт почтовых ящиков".</span><span class="sxs-lookup"><span data-stu-id="16eb0-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="16eb0-107">Дополнительные сведения см. в статье [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="16eb0-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
