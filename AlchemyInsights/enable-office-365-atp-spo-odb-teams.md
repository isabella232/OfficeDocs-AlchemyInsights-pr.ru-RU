---
title: Включение пакета Office 365 ATP для SharePoint, OneDrive и Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703439"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Включение расширенной защиты от угроз для Office 365 для SharePoint Online, OneDrive и Microsoft Teams

1. Перейдите на https://protection.office.com и войдите.
2. Выберите пункт**безопасные вложения** > **политики** >  **управления угрозами**.
3. Выберите **включить ATP для SharePoint, OneDrive и Microsoft Teams**, а затем нажмите кнопку **сохранить**.
4. Предложен В качестве глобального администратора или администратора SharePoint Online выполните командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с параметром **дисалловинфектедфиледовнлоад** , для которого задано *значение true*.
5. Предложен [Настройка оповещений](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) об обнаруженных файлах.

> [!NOTE]
> Служба ATP будет сканировать каждый отдельный файл в SharePoint Online, OneDrive или Microsoft Teams. Файлы сканируются асинхронно, с помощью процесса, использующего общие и гостевые события, вместе с интеллектуальными эвристиками и сигналами угроз для идентификации вредоносных файлов. Просмотреть [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).