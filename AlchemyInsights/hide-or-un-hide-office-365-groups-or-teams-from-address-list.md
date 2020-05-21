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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="335ee-102">Скрытие и отображение групп или команд Office 365 в списке адресов</span><span class="sxs-lookup"><span data-stu-id="335ee-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="335ee-103">Используйте следующую команду PowerShell EXO, чтобы скрыть или отобразить группы или команды Office 365 в списке адресов (GAL) клиентов Exchange (Outlook, OWA).</span><span class="sxs-lookup"><span data-stu-id="335ee-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="335ee-104">Используйте следующую команду PowerShell EXO, чтобы скрыть или отобразить группы или команды Office 365 в клиентах Exchange (Outlook, OWA).</span><span class="sxs-lookup"><span data-stu-id="335ee-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="335ee-105">Подробные инструкции см. в статье [Скрытие групп Office 365 в глобальном списке адресов и в клиентах Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="335ee-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
