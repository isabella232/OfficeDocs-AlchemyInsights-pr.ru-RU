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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552522"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams

1. Используя учетные данные глобального администратора или администратора безопасности, войдите в Центр безопасности и соответствия требованиям [Office 365.](https://protection.office.com/)
2. Выберите **управление угрозами** в левой области, а затем выберите **вложения Policy**  >  [Safe.](https://protection.office.com/safeattachment)
3. **Включите Microsoft Defender для Office 365 для SharePoint, OneDrive** и Microsoft Teams, а затем выберите **Сохранить**.
    > [!TIP]
    >
    > - В качестве глобального администратора или администратора SharePoint Online запустите следующий комдлет PowerShell с параметром **DisallowInfectedFileDownload,** заданным для *true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Настройка оповещений для обнаруженных файлов](https://go.microsoft.com/fwlink/?linkid=2092110)

Дополнительные сведения см. [в разделе Microsoft Defender for Office 365 для SharePoint, OneDrive и Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
