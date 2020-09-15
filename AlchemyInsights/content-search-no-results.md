---
title: Поиск контента без результатов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680660"
---
# <a name="no-results-from-content-searchexports"></a>Нет результатов из поиска и экспортов контента

Проблемы с поиском контента и экспортами не возвращают данные могут быть вызваны определенным администратором и не взаимодействующими со всеми администраторами.

Чтобы устранить эту проблему, проверьте наличие фильтров безопасности соответствия, которые могут привести к этому.
1. Подключение к PowerShell центра безопасности и соответствия требованиям
2. Выполните следующую команду командлеты:
<br>$org = "yourdomain.com"
<br>Get – ComplianceSecurityFilter — организация $org