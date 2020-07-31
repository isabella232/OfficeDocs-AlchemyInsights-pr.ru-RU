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
# <a name="pausing-scheduled-updates"></a>Приостановка запланированных обновлений

При вводе команды pause устройства не обрабатывают команду до своего следующего входа в Intune. В связи с этим ваши устройства могут:

- установить запланированные обновления до очередного входа.
- быть отключены от сети в тот момент, когда вы ввели команду pause. В этом случае, если устройства были включены, они могли скачать и установить запланированные обновления до очередного входа.