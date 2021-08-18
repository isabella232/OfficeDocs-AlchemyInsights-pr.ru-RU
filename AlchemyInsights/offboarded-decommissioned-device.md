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
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324457"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Проблемы с удалением отключенного или списанного устройства из инвентаризации устройств

Microsoft Defender для конечной точки в настоящее время не позволяет вручную удалять запись устройства с отключенного или списанного устройства из инвентаризации устройств.

В целях безопасности устройство остается на портале в качестве исторической записи на срок до 180 дней. Однако данные устройства будут сгвеяться в соответствии с настроенным периодом хранения.

**Примечание:** Отключенное или списаное устройство автоматически переключается в состояние **Неактивно** через семь дней. Кроме того, устройства, не активные в течение последних 30 дней, не будут учитываться в данных, отражающих оценку контроль угроз и уязвимостей или Microsoft Secure Score для устройств.
 
Если вы по-прежнему не хотите видеть определенные устройства в представлении инвентаризации устройств, попробуйте поместить тег устройства, чтобы отфильтровать списанное устройство из представления инвентаризации устройств.

Дополнительные сведения см. в указанных ниже статьях.

[Offboard devices from the Microsoft Defender for Endpoint service](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Оценка экспозиции в контроль угроз и уязвимостей](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Исправление нездоровых датчиков в Microsoft Defender для конечной точки](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Эффективное использование тегов (часть 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Эффективное использование тегов (часть 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Эффективное использование тегов (часть 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




