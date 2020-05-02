---
title: MC210173 — прекращение поддержки функции создания настраиваемой формы SharePoint Designer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928540"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 — прекращение поддержки функции создания настраиваемой формы SharePoint Designer

Мы выявили проблему, влияющую на функцию SharePoint Designer для [создания настраиваемых форм](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) в SharePoint Online. После тщательного изучения мы определили, что для этой проблемы не существует известного исправления, и мы решили отключить функцию создания настраиваемой формы с 3:00 (UTC) 25 апреля 2020 г. (суббота). Это изменение не повлияет на возможность изменения ранее созданных форм или на другие имеющиеся функции в SharePoint Online Designer.

После внесения этого изменения пользователи могли получать сообщение об ошибке "Не удалось сохранить изменения списка на сервере" при создании форм.

Пользователи, ранее применявшие SharePoint Designer для создания настраиваемых форм, могут для этой цели использовать [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

PowerApps — это простой и мощный инструмент, позволяющий пользователям, которые работают в современном интерфейсе SharePoint Online, создавать и редактировать настраиваемые формы для списков и библиотек документов SharePoint прямо в окне браузера. PowerApps не требует традиционных знаний для написания кода или скачивания дополнительных приложений, таких как InfoPath.

**Примечание**. Пользователям классической версии SharePoint Online потребуется временно отключить современный интерфейс для доступа к PowerApps и его использования. Но все настраиваемые формы, созданные в PowerApps доступны в классическом интерфейсе SharePoint Online.