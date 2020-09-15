---
title: Приостановка запланированных обновлений
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721568"
---
# <a name="pausing-scheduled-updates"></a>Приостановка запланированных обновлений

При вводе команды pause устройства не обрабатывают команду до своего следующего входа в Intune. В связи с этим ваши устройства могут:

- установить запланированные обновления до очередного входа.
- быть отключены от сети в тот момент, когда вы ввели команду pause. В этом случае, если устройства были включены, они могли скачать и установить запланированные обновления до очередного входа.