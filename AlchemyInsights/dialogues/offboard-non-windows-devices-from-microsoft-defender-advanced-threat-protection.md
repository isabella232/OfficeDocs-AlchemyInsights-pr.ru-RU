---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530217"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)

Вот как это сделать:

1. Следуйте документации сторонних сторон для отключения сторонних решений от ATP Защитника Майкрософт.
2. В клиенте Azure Active Directory удалите разрешения на стороннее решение:

    1. Войдите на [портал Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Выберите **все службы**  >  **Azure Active Directory**  >  **Корпоративные приложения.**
    1. Выберите приложение, которое вы хотите отключить.
    1. Выберите **Удалить**.

Подробнее см. в таблице [Offboard non-Windows devices.](https://go.microsoft.com/fwlink/?linkid=2143630)
