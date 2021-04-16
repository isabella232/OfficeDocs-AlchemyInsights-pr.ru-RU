---
title: Средство экспорта обнаруженных электронных данных
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814601"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не можете установить или запустить средство экспорта электронных обнаружений?

Если вы не можете установить или запустить средство экспорта электронных открытий для скачивания результатов поиска, проверьте следующие вещи:
  
- Компьютер, на который вы используете, соответствует этим предварительным требованиям:

  - 32- или 64-разрядный выпуск Windows 7 и более поздней версии.




  - Microsoft .NET Framework 4.7

  - Поддерживаемый браузер:

  - Microsoft Edge

    Или

  - Internet Explorer 10 и более поздние версии.

    Другие браузеры, такие как Google Chrome и Mozilla Firefox, не поддерживаются.

- Ваша организация может подключиться к конечной точке Azure, которая является **\* .blob.core.windows.net** (под диктовка представляет уникальный идентификатор для экспортной работы).

- Вам назначена роль экспорта в Центре соответствия требованиям безопасности Microsoft 365. &amp; По умолчанию эта роль назначена только группе ролей диспетчера электронных обнаружений. См. [назначение разрешений на открытие электронной почты.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Дополнительные сведения см. в [результатах поиска по экспорту контента.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Если вы экспортируете более 100 000 почтовых ящиков, для скачивания результатов Экспорта: Экспорт результатов из более  [чем 100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)почтовых ящиков необходимо использовать следующие powershell.