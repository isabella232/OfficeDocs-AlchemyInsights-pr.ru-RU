---
title: ATP для SharePoint, OneDrive и Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715574"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP для SharePoint, OneDrive и Microsoft Teams

Выполните следующие действия, чтобы включить расширенную защиту от угроз.

1. Перейдите к [https://protection.office.com](https://protection.office.com) учетной записи глобального администратора или администратора безопасности и войдите в нее.

2. В левой области навигации в разделе **Управление угрозами**выберите **Policy** пункт \> **безопасные вложения**политики.

3. Выберите **включить ATP для SharePoint, OneDrive и Microsoft Teams**.

4. [Создайте политику оповещений о действиях](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) для получения уведомлений при обнаружении вредоносных файлов.

Подробные инструкции приведены в этой [статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Примечание**: по дизайну ATP не сканирует каждый отдельный файл в SharePoint Online, OneDrive для бизнеса или Microsoft Teams. Файлы отсканированы асинхронно процессом, который использует операции общего доступа, гостевые действия и сигналы угроз для идентификации вредоносных файлов. Дополнительные сведения см. в этой [статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
