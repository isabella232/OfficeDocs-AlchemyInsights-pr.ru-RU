---
title: Поиск контента Без результатов
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816861"
---
# <a name="no-results-from-content-searchexports"></a>Нет результатов поиска и экспорта контента

Проблемы с поиском и экспортом контента, не возвращая данные, могут быть вызваны определенным фильтром безопасности соответствия требованиям, который был настроен определенным администратором и не передает их всем администраторам.

Чтобы устранить это, проверьте, существуют ли фильтры безопасности соответствия требованиям, которые могут вызывать это:
1. Подключение к Центру безопасности и соответствия требованиям Powershell
2. Запустите следующие команды:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org