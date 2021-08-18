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
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090166"
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

> [!NOTE]
> Это не будет работать для комбинаций лицензий, таких как: Win E5 + O365 E5 + EMS E5. Чтобы настроить эту функцию, необходимо иметь чистую лицензию M365 E5.

Дополнительные сведения о лицензировании DLP конечной точки см. в таблице [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
