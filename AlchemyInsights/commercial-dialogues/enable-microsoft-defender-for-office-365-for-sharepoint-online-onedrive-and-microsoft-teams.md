---
title: Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058879"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams

1. Используя учетные данные глобального администратора или администратора безопасности, войдите в центр Office 365 [безопасности и соответствия](https://protection.office.com/)требованиям.
2. Выберите **управление угрозами** в левой области, а затем   >  [выберите Сейф политики.](https://protection.office.com/safeattachment)
3. Включите Microsoft Defender для Office 365 **для SharePoint, OneDrive и Microsoft Teams,** а затем выберите **Сохранить**.
    > [!TIP]
    >
    > - В качестве глобального администратора или администратора SharePoint Online запустите следующий комдлет PowerShell с параметром **DisallowInfectedFileDownload,** установленным для true *:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Настройка оповещений для обнаруженных файлов](https://go.microsoft.com/fwlink/?linkid=2092110)

Дополнительные сведения см. в Office 365 Microsoft [Defender для SharePoint, OneDrive и Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
