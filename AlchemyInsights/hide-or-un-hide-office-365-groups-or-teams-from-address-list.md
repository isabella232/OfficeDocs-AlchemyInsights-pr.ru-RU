---
title: Скрытие и отображение групп или команд Office 365 в списке адресов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225449"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Скрытие и отображение групп или команд Office 365 в списке адресов

Используйте следующую команду PowerShell EXO, чтобы скрыть или отобразить группы или команды Office 365 в списке адресов (GAL) клиентов Exchange (Outlook, OWA).

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Используйте следующую команду PowerShell EXO, чтобы скрыть или отобразить группы или команды Office 365 в клиентах Exchange (Outlook, OWA).

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Подробные инструкции см. в статье [Скрытие групп Office 365 в глобальном списке адресов и в клиентах Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
