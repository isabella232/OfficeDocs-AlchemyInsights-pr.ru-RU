---
title: Проблемы с удалением отключенного или списанного устройства из инвентаризации устройств
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319181"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="17d32-102">Проблемы с удалением отключенного или списанного устройства из инвентаризации устройств</span><span class="sxs-lookup"><span data-stu-id="17d32-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="17d32-103">Microsoft Defender для конечной точки в настоящее время не позволяет вручную удалять запись устройства с отключенного или списанного устройства из инвентаризации устройств.</span><span class="sxs-lookup"><span data-stu-id="17d32-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="17d32-104">В целях безопасности устройство остается на портале в качестве исторической записи на срок до 180 дней.</span><span class="sxs-lookup"><span data-stu-id="17d32-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="17d32-105">Однако данные устройства будут сгвеяться в соответствии с настроенным периодом хранения.</span><span class="sxs-lookup"><span data-stu-id="17d32-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="17d32-106">**Примечание:** Отключенное или списаное устройство автоматически переключается в состояние **Неактивно** через семь дней.</span><span class="sxs-lookup"><span data-stu-id="17d32-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="17d32-107">Кроме того, устройства, не активные в течение последних 30 дней, не будут учитываться в данных, отражающих оценку подверженности угрозам организации и уязвимостям или microsoft Secure Score для устройств.</span><span class="sxs-lookup"><span data-stu-id="17d32-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="17d32-108">Если вы по-прежнему не хотите видеть определенные устройства в представлении инвентаризации устройств, попробуйте поместить тег устройства, чтобы отфильтровать списанное устройство из представления инвентаризации устройств.</span><span class="sxs-lookup"><span data-stu-id="17d32-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="17d32-109">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="17d32-109">For more information, see:</span></span>

[<span data-ttu-id="17d32-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="17d32-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="17d32-111">Оценка экспозиции в управлении угрозами и уязвимостью</span><span class="sxs-lookup"><span data-stu-id="17d32-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="17d32-112">Исправление нездоровых датчиков в Microsoft Defender для конечной точки</span><span class="sxs-lookup"><span data-stu-id="17d32-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="17d32-113">Эффективное использование тегов (часть 1)</span><span class="sxs-lookup"><span data-stu-id="17d32-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="17d32-114">Эффективное использование тегов (часть 2)</span><span class="sxs-lookup"><span data-stu-id="17d32-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="17d32-115">Эффективное использование тегов (часть 3)</span><span class="sxs-lookup"><span data-stu-id="17d32-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




