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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058015"
---
# <a name="no-results-from-content-searchexports"></a>Нет результатов поиска и экспорта контента

Проблемы с поиском и экспортом контента, не возвращая данные, могут быть вызваны определенным фильтром безопасности соответствия требованиям, который был настроен определенным администратором и не передает их всем администраторам.

Чтобы устранить это, проверьте, существуют ли фильтры безопасности соответствия требованиям, которые могут вызывать это:
1. Подключение центра безопасности и соответствия требованиям Powershell
2. Запустите следующие команды:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org