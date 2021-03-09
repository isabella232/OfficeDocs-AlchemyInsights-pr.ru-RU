---
title: Исправление правил транспорта
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568682"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="1bee2-102">Исправление правил транспорта</span><span class="sxs-lookup"><span data-stu-id="1bee2-102">Fix transport rules</span></span>

<span data-ttu-id="1bee2-103">На это сообщение повлияло правило пользовательского потока почты.</span><span class="sxs-lookup"><span data-stu-id="1bee2-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="1bee2-104">Чтобы просмотреть точное правило, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="1bee2-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="1bee2-105">В результатах отправки в **статье Дополнительные сведения** обратите внимание на **GUID** или **имя политики.**</span><span class="sxs-lookup"><span data-stu-id="1bee2-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="1bee2-106">Запуск оболочки управления Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bee2-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="1bee2-107">Дополнительные сведения см. в [рублях Open the Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="1bee2-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="1bee2-108">Запустите эту команду (с помощью GUID из отправки): **Get-TransportRule -identity "GUID"** | fl \* Description\*</span><span class="sxs-lookup"><span data-stu-id="1bee2-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="1bee2-109">Просмотрите описание, чтобы просмотреть настроенные условия, которые повлияли на сообщение.</span><span class="sxs-lookup"><span data-stu-id="1bee2-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="1bee2-110">Дополнительные дополнительные информации [см. в см. в ленте Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="1bee2-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
