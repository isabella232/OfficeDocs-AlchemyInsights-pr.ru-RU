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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666653"
---
# <a name="no-results-returned-during-content-searchexport"></a>Результаты поиска и экспорта контента не возвращаются

Если у вас возникли проблемы со следующими сценариями eDiscovery:

- Поиск и экспорт контента не возвращают данных или непредвиденных данных
- Не удается найти или экспортировать eDiscovery

Это может быть вызвано определенными фильтрами безопасности соответствия требованиям, которые были настроены определенным администратором и не были донесы до всех администраторов.

Чтобы устранить эту проблему, проверьте, есть ли какие-либо фильтры соответствия требованиям безопасности, которые могут быть причиной таких проблем:

1. Подключение к Powershell Центра безопасности и соответствия требованиям
2. Запустите следующие командлеты:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Дополнительные сведения о фильтрах безопасности соответствия требованиям см. в фильтрации разрешений [для поиска контента](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
