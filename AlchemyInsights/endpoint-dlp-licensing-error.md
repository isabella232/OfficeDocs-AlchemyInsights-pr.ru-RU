---
title: Ошибка лицензирования защиты от потери данных в конечной точке
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477702"
---
# <a name="endpoint-dlp-licensing-error"></a>Ошибка лицензирования защиты от потери данных в конечной точке

При попытке настроить DLP для конечной точки при получении следующего сообщения об ошибке:

`Your organization is missing the licenses required to manage these devices`.

Убедитесь, что у вас есть одна из следующих подписок или надстроек:

- Microsoft 365 E5
- Microsoft 365 A5 (для учебных заведений)
- Соответствие требованиям Microsoft 365 E5
- Соответствие требованиям Microsoft 365 A5
- Защита информации и управление данными в Microsoft 365 E5
- Защита информации и управление данными в Microsoft 365 A5

> [!NOTE]
> Эта проблема не будет работать для таких комбинаций лицензий, как: Win/O365, а затем EMS. Чтобы настроить эту функцию, необходимо иметь чистую лицензию M365.

Дополнительные сведения о лицензировании DLP в конечной точке приведены в разделе [Лицензирование DLP конечной точки.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
