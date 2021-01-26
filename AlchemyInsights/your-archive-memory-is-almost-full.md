---
title: Архивный почтовый ящик почти заполнен
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950515"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="168f1-102">Архивный почтовый ящик почти заполнен</span><span class="sxs-lookup"><span data-stu-id="168f1-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="168f1-103">Если пользователь получает предупреждение; **Архивный почтовый ящик** почти заполнен, или вам нужно увеличить размер архивного почтового ящика, вот несколько советов:</span><span class="sxs-lookup"><span data-stu-id="168f1-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="168f1-104">Если пользователю назначена лицензия Exchange Online (план 1), обновим лицензию на **Exchange Online (план 2),** чтобы увеличить размер с 50 ГБ до 100 ГБ.</span><span class="sxs-lookup"><span data-stu-id="168f1-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="168f1-105">Если пользователю уже назначена любая из следующих надстроек: **Exchange Online (план 2)** или Exchange Online (план 1) с надстройка архивация на базе Exchange Online, воспользуйтесь следующими действиями для автоматического расширения архивов.</span><span class="sxs-lookup"><span data-stu-id="168f1-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="168f1-106">[Подключись к Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="168f1-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="168f1-107">Запустите следующий командлет для пользователя:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="168f1-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="168f1-108">Чтобы подтвердить, что он включен для пользователя, запустите следующий командлет:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="168f1-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="168f1-109">Дополнительные сведения см. в указанных ниже статьях.    </span><span class="sxs-lookup"><span data-stu-id="168f1-109">For more information see:</span></span>

- [<span data-ttu-id="168f1-110"> Включить неограниченный архив — справка для администраторов - Соответствие требованиям Microsoft 365 | Документы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="168f1-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="168f1-111">Ограничения Exchange Online — описание службы | Документы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="168f1-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="168f1-112">Обновление до другой бизнес-| Документы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="168f1-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

