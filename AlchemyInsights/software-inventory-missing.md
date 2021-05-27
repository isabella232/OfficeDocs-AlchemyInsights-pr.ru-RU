---
title: Перечень программного обеспечения отсутствует или неточен
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658058"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="ce66c-102">Перечень программного обеспечения отсутствует или неточен</span><span class="sxs-lookup"><span data-stu-id="ce66c-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="ce66c-103">Инвентаризация программного обеспечения в управлении угрозами и уязвимостями (TVM) — это список программ, применяемых в организации, который составляется с помощью формального Common Platform Enumerations (CPE, список типовых платформ).</span><span class="sxs-lookup"><span data-stu-id="ce66c-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="ce66c-104">Сведения об уязвимостях программных продуктов без формального CPE отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ce66c-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="ce66c-105">Инвентаризация также включает такие сведения, как имя поставщика, количество слабых мест, угроз и количество подверженных воздействию устройств.</span><span class="sxs-lookup"><span data-stu-id="ce66c-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="ce66c-106">Изменения программного обеспечения на устройствах обычно отображаются на порталах безопасности в течение двух часов.</span><span class="sxs-lookup"><span data-stu-id="ce66c-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="ce66c-107">Однако иногда это может занять больше времени.</span><span class="sxs-lookup"><span data-stu-id="ce66c-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="ce66c-108">В настоящее время не существует способа принудительной синхронизации; оценка является постоянной и непрекращающейся.</span><span class="sxs-lookup"><span data-stu-id="ce66c-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="ce66c-109">Если вы вносили изменения в программное обеспечение, которые неточно отобразились в TVM через 5 часов, выполните описанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="ce66c-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="ce66c-110">Чтобы понять, как было обнаружено программное обеспечение, ознакомьтесь с разделом свидетельств программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="ce66c-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="ce66c-111">Убедитесь, что необходимое программное обеспечение поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce66c-111">Make sure that the software is supported.</span></span> <span data-ttu-id="ce66c-112">Программное обеспечение может быть видимым только на уровне устройства, даже если в настоящее время на нем не активирован контроль угроз и уязвимостей.</span><span class="sxs-lookup"><span data-stu-id="ce66c-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="ce66c-113">Однако доступны только ограниченные данные.</span><span class="sxs-lookup"><span data-stu-id="ce66c-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="ce66c-114">Ознакомьтесь с инструкциями по отправке отчета о неточности на портале в разделе [отчете о неточности](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="ce66c-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="ce66c-115">**Примечание**. Отчеты о неточности с портала MDE — это односторонний канал связи с разработчиками.</span><span class="sxs-lookup"><span data-stu-id="ce66c-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="ce66c-116">Если проблема является срочной, отправьте запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="ce66c-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="ce66c-117">Подробнее см. в статье [Инвентаризация программного обеспечения: контроль угроз и уязвимостей](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="ce66c-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>