---
title: Результаты, возвращенные во время поиска и экспорта контента, не возвращаются
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101279"
---
# <a name="no-results-returned-during-content-searchexport"></a>Результаты, возвращенные во время поиска и экспорта контента, не возвращаются

Если возникли проблемы со следующими сценариями по обнаружению электронных обнаружений:

- Поиск и экспорт контента не возвращают данных или неожиданных данных
- Поиск и экспорт электронной почты не удается

Это может быть связано с определенными фильтрами безопасности соответствия требованиям, которые были настроены определенным администратором и не были доведены до всех администраторов.

Чтобы устранить эту проблему, проверьте, существуют ли фильтры безопасности соответствия требованиям, которые могут вызывать эти проблемы:

1. Подключение центра безопасности и соответствия требованиям Powershell
2. Запустите следующие команды:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Дополнительные сведения о фильтрах безопасности соответствия см. в материалах [Permissions Filtering for Content Search.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
