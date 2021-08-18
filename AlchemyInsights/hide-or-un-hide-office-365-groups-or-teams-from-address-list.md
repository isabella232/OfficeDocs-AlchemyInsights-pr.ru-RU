---
title: Скрытие и отображение групп или команд Office 365 в списке адресов
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088409"
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
