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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="c6984-102">Пакет переноса общедоступных папок со статусом CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="c6984-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="c6984-103">Чтобы выполнить пакет, выполните следующие действия, пропустив крупные и плохие элементы:</span><span class="sxs-lookup"><span data-stu-id="c6984-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="c6984-104">Утверждение пропущенных элементов в пакете миграции:</span><span class="sxs-lookup"><span data-stu-id="c6984-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="c6984-105">Используйте следующую команду для утверждения пропущенных элементов в запросах на миграцию, которые "синхронизированы", но не завершены:</span><span class="sxs-lookup"><span data-stu-id="c6984-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="c6984-106">Пакет миграции и запросы должны возобновиться и завершиться в течение нескольких минут.</span><span class="sxs-lookup"><span data-stu-id="c6984-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

