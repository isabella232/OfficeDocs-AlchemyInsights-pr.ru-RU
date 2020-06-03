---
title: ATP для SharePoint, OneDrive и Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508425"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP для SharePoint, OneDrive и Microsoft Teams

Выполните следующие действия, чтобы включить расширенную защиту от угроз.

1. Перейдите к [https://protection.office.com](https://protection.office.com) учетной записи глобального администратора или администратора безопасности и войдите в нее.

2. В левой области навигации в разделе **Управление угрозами**выберите **Policy** пункт \> **безопасные вложения**политики.

3. Выберите **включить ATP для SharePoint, OneDrive и Microsoft Teams**.

4. [Создайте политику оповещений о действиях](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) для получения уведомлений при обнаружении вредоносных файлов.

Подробные инструкции приведены в этой [статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Примечание**: по дизайну ATP не сканирует каждый отдельный файл в SharePoint Online, OneDrive для бизнеса или Microsoft Teams. Файлы отсканированы асинхронно процессом, который использует операции общего доступа, гостевые действия и сигналы угроз для идентификации вредоносных файлов. Дополнительные сведения см. в этой [статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
