---
title: DLP конечной точки не развернута на устройстве пользователя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 56783b007b5eebc7ca671247f24f5b513b9d8f5c321f59a63170425c2d376a94
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900261"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP конечной точки не развернута на устройстве пользователя

Если параметр защиты от потери данных (DLP) конечной точки не применен на устройстве пользователя, нужно подтвердить соответствие этим требованиям:

- На устройстве установлена Windows 10 x64 сборки 1809 или более поздняя версия.
- Установлен клиент для защиты от вредоносных программ версии 4.18.2009.7 или более поздней версии.
- Устройство является **одним** из следующих:
    
    - С присоединением к Azure Active Directory (Azure AD)
    - С гибридным присоединением к Azure AD
    - С регистрацией в AAD

- Чтобы применить действие политики, убедитесь в том, что браузер Microsoft Chromium Edge установлен на устройстве с конечной точкой.

Дополнительные требования к развертыванию защиты от потери данных в конечной точке см. в разделе[. Начало работы с функцией защиты от потери данных](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).