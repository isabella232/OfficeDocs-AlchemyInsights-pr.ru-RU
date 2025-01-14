---
title: Включить Office 365 atP для SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332172"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Включить Microsoft Defender для Office 365 для SharePoint Online, OneDrive и Microsoft Teams

1. Перейдите на https://protection.office.com и войдите.
2. Выберите **политику управления**  >    >  **угрозами Сейф вложения.**
3. Выберите **Включить Защитник для Office 365 для SharePoint, OneDrive и Microsoft Teams,** а затем нажмите **кнопку Сохранить**.
4. (Рекомендуется) В качестве глобального администратора или администратора SharePoint Online запустите комлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с параметром **DisallowInfectedFileDownload,** заданным для *true*.
5. (Рекомендуется) [Настройка оповещений](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для обнаруженных файлов.

**Примечание.** Microsoft Defender для Office 365 не будет сканировать каждый файл SharePoint Online, OneDrive или Microsoft Teams. Файлы сканируют асинхронно, с помощью процесса, который использует события совместной и гостевой активности, а также интеллектуальные heuristics и сигналы угрозы для выявления вредоносных файлов. См. в Office 365 [Microsoft Defender для SharePoint, OneDrive и Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
