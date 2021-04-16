---
title: Пакет переноса общедоступных папок со статусом CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812477"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Пакет переноса общедоступных папок со статусом CompletedWithErrors

Чтобы выполнить пакет, выполните следующие действия, пропустив крупные и плохие элементы: 
1. Утверждение пропущенных элементов в пакете миграции:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Используйте следующую команду для утверждения пропущенных элементов в запросах на миграцию, которые "синхронизированы", но не завершены:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Пакет миграции и запросы должны возобновиться и завершиться в течение нескольких минут.

