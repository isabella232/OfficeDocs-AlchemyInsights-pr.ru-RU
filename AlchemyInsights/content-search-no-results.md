---
title: Поиск контента без результатов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800554"
---
# <a name="no-results-from-content-searchexports"></a>Нет результатов из поиска и экспортов контента

Проблемы с поиском контента и экспортами не возвращают данные могут быть вызваны определенным администратором и не взаимодействующими со всеми администраторами.

Чтобы устранить эту проблему, проверьте наличие фильтров безопасности соответствия, которые могут привести к этому.
1. Подключение к PowerShell центра безопасности и соответствия требованиям
2. Выполните следующую команду командлеты:
<br>$org = "yourdomain.com"
<br>Get – ComplianceSecurityFilter — организация $org