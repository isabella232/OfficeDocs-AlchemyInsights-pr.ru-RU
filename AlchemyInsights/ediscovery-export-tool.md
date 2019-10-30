---
title: Средство экспорта обнаруженных электронных данных
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 7e2964ef0a44ddf421e4aae007acbdbda196e20f
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769316"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не удается установить или запустить средство экспорта обнаружения электронных данных?

Если вы не можете установить или запустить средство экспорта eDiscovery Office 365 для загрузки результатов поиска, проверьте следующие моменты.
  
- Компьютер, который вы используете, соответствует этим предварительным требованиям:

  - 32- или 64-разрядный выпуск Windows 7 и более поздней версии.




  - Microsoft .NET Framework 4,7

  - Поддерживаемый браузер:

  - Microsoft Edge

    или

  - Internet Explorer 10 и более поздние версии.

    Другие браузеры, такие как Google Chrome и Mozilla Firefox, не поддерживаются.

- Ваша организация может подключаться к конечной точке в Azure, т ** \*. е. BLOB.Core.Windows.NET** (подстановочный знак представляет уникальный идентификатор задания экспорта).

- Роль экспорта назначена в центре безопасности &amp; и соответствия требованиям Office 365. По умолчанию эта роль назначается только группе ролей диспетчера обнаружения электронных данных. См. [Назначение разрешений на обнаружение электронных](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions)данных.

Дополнительные сведения можно найти в статье [Экспорт результатов поиска контента](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  