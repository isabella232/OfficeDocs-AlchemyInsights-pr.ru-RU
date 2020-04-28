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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908357"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Скрытие списка адресов (GAL) группы Microsoft 365

Чтобы скрыть группу Microsoft 365 из списков адресов (GAL) клиентов Exchange (например, Outlook или OWA), выполните следующую команду в командной консоли EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Чтобы скрыть группу Microsoft 365, видимую для клиентов Exchange, используйте следующую команду в командной консоли EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

