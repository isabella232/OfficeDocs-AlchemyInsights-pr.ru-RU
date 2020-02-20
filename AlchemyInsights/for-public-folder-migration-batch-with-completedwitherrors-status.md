---
title: Для пакета миграции общедоступных папок с состоянием Комплетедвисеррорс
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158632"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Для пакета миграции общедоступных папок с состоянием Комплетедвисеррорс

Выполните следующие действия, чтобы завершить пакет, пропуская крупные или поврежденные элементы: 
1. Утвердите пропущенные элементы в пакете миграции:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Используйте следующую команду, чтобы утвердить пропущенные элементы в запросах на миграцию, которые были синхронизированы, но не выполнены.

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Пакеты миграции и запросы должны возобновляться и завершаться через несколько минут.

