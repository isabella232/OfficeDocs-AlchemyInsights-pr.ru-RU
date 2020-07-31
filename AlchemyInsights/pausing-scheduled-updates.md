---
title: Приостановка запланированных обновлений
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530596"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="dc9b6-102">Приостановка запланированных обновлений</span><span class="sxs-lookup"><span data-stu-id="dc9b6-102">Pausing scheduled updates</span></span>

<span data-ttu-id="dc9b6-103">При вводе команды pause устройства не обрабатывают команду до своего следующего входа в Intune.</span><span class="sxs-lookup"><span data-stu-id="dc9b6-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="dc9b6-104">В связи с этим ваши устройства могут:</span><span class="sxs-lookup"><span data-stu-id="dc9b6-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="dc9b6-105">установить запланированные обновления до очередного входа.</span><span class="sxs-lookup"><span data-stu-id="dc9b6-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="dc9b6-106">быть отключены от сети в тот момент, когда вы ввели команду pause.</span><span class="sxs-lookup"><span data-stu-id="dc9b6-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="dc9b6-107">В этом случае, если устройства были включены, они могли скачать и установить запланированные обновления до очередного входа.</span><span class="sxs-lookup"><span data-stu-id="dc9b6-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>