---
title: Инструкции по скрытию и скрытию списка адресов групп из списка
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580022"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Скрытие списка адресов (GAL) группы Microsoft 365

Чтобы скрыть группу Microsoft 365 из списков адресов (GAL) клиентов Exchange (например, Outlook или OWA), выполните следующую команду в командной консоли EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Чтобы скрыть группу Microsoft 365, видимую для клиентов Exchange, используйте следующую команду в командной консоли EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

