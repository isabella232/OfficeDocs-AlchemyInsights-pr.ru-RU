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
ms.openlocfilehash: 6352603a391ddcb44d2728c7587bf15a6cd97ebb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507183"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не удается установить или запустить средство экспорта обнаружения электронных данных?

Если вы не можете установить или запустить средство экспорта eDiscovery для загрузки результатов поиска, проверьте следующие моменты.
  
- Компьютер, который вы используете, соответствует этим предварительным требованиям:

  - 32- или 64-разрядный выпуск Windows 7 и более поздней версии.




  - Microsoft .NET Framework 4,7

  - Поддерживаемый браузер:

  - Microsoft Edge

    ИЛИ

  - Internet Explorer 10 и более поздние версии.

    Другие браузеры, такие как Google Chrome и Mozilla Firefox, не поддерживаются.

- Ваша организация может подключаться к конечной точке в Azure, т ** \* . е. BLOB.Core.Windows.NET** (подстановочный знак представляет уникальный идентификатор задания экспорта).

- Вы назначили роль экспорт в центре безопасности Майкрософт 365 &amp; . По умолчанию эта роль назначается только группе ролей диспетчера обнаружения электронных данных. См. [Назначение разрешений на обнаружение электронных](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)данных.

Дополнительные сведения можно найти в статье [Экспорт результатов поиска контента](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  