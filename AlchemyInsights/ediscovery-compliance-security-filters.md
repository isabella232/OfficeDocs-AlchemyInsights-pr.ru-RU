---
title: Результаты поиска и экспорта контента не возвращаются
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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727236"
---
# <a name="no-results-returned-during-content-searchexport"></a>Результаты поиска и экспорта контента не возвращаются

Если у вас возникли проблемы со следующими сценариями eDiscovery:

- Поиск и экспорт контента не возвращают данных или непредвиденных данных
- Не удается найти или экспортировать eDiscovery

Это может быть вызвано определенными фильтрами безопасности соответствия требованиям, которые были настроены определенным администратором и не были оадминистрироваться всем администраторам.

Чтобы устранить эту проблему, проверьте, есть ли фильтры соответствия требованиям безопасности, которые могут быть причиной таких проблем:

1. Подключение к Powershell Центра безопасности и соответствия требованиям
2. Запустите следующие командлеты:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Дополнительные сведения о фильтрах безопасности соответствия требованиям см. в подкассылной области ["Фильтрация разрешений для поиска контента"](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
