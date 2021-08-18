---
title: Ошибка лицензирования DLP конечной точки
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322144"
---
# <a name="endpoint-dlp-licensing-error"></a>Ошибка лицензирования DLP конечной точки

При попытке настроить DLP конечной точки, если вы получаете следующую ошибку:

`Your organization is missing the licenses required to manage these devices`.

Убедитесь, что у вас есть одна из следующих подписок или надстройок:

- Microsoft 365 E5
- Microsoft 365 A5 (для учебных заведений)
- Соответствие требованиям Microsoft 365 E5
- Соответствие требованиям Microsoft 365 A5
- Защита информации и управление данными в Microsoft 365 E5
- Защита информации и управление данными в Microsoft 365 A5

**Примечание.** Это не будет работать для комбинаций лицензий, таких как: Win E5 + O365 E5 + EMS E5. Чтобы настроить эту функцию, необходимо иметь чистую лицензию M365 E5.

Дополнительные сведения о лицензировании DLP конечной точки см. в таблице [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
