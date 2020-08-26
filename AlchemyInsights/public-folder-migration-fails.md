---
title: Сбой миграции общедоступной папки на уровне 95 %
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903606"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="cf1c8-102">Сбой миграции общедоступной папки на уровне 95 %</span><span class="sxs-lookup"><span data-stu-id="cf1c8-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="cf1c8-103">При сбое миграции общедоступных папок на уровне 95% с ошибкой FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="cf1c8-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="cf1c8-104">Скачайте и запустите сценарий [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) на локальном сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf1c8-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="cf1c8-105">Выполните действия по исправлению, предлагаемые сценарием.</span><span class="sxs-lookup"><span data-stu-id="cf1c8-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="cf1c8-106">Выполните команду Sync-MailPublicFolders (для Exchange 2010) или Sync-ModernMailPublicFolders (для Exchange 2013 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cf1c8-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="cf1c8-107">Возобновите миграцию общедоступной папки.</span><span class="sxs-lookup"><span data-stu-id="cf1c8-107">Resume public folder migration.</span></span>
