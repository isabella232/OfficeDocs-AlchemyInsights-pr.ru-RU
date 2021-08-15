---
title: Offboard non-Windows от Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967814"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-Windows от Microsoft Defender Advanced Threat Protection (ATP)

Вот как это сделать:

1. Следуйте документации сторонних сторон для отключения сторонних решений от ATP Защитника Майкрософт.
2. От Azure Active Directory клиента удалите разрешения для сторонного решения:

    1. Войдите на [портал Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Выберите **все**  >  **службы Azure Active Directory** Enterprise  >  **приложения**.
    1. Выберите приложение, которое вы хотите отключить.
    1. Нажмите **Удалить**.

Дополнительные дополнительные информации см. в [таблице Offboard non-Windows устройств.](https://go.microsoft.com/fwlink/?linkid=2143630)
