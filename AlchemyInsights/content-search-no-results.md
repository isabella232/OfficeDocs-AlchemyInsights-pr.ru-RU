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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516792"
---
# <a name="no-results-from-content-searchexports"></a>Нет результатов из поиска и экспортов контента

Проблемы с поиском контента и экспортами не возвращают данные могут быть вызваны определенным администратором и не взаимодействующими со всеми администраторами.

Чтобы устранить эту проблему, проверьте наличие фильтров безопасности соответствия, которые могут привести к этому.
1. Подключение к PowerShell центра безопасности и соответствия требованиям
2. Выполните следующую команду командлеты:
<br>$org = "yourdomain.com"
<br>Get – ComplianceSecurityFilter — организация $org