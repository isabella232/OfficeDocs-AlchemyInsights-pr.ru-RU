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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043613"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="0c0aa-102">Для пакета миграции общедоступных папок с состоянием Комплетедвисеррорс</span><span class="sxs-lookup"><span data-stu-id="0c0aa-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="0c0aa-103">Выполните следующие действия, чтобы завершить пакет, пропуская крупные или поврежденные элементы:</span><span class="sxs-lookup"><span data-stu-id="0c0aa-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="0c0aa-104">Утвердите пропущенные элементы в пакете миграции:</span><span class="sxs-lookup"><span data-stu-id="0c0aa-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="0c0aa-105">Set — MigrationBatch \<BatchName> аппровескиппедитемс</span><span class="sxs-lookup"><span data-stu-id="0c0aa-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="0c0aa-106">Используйте следующую команду, чтобы утвердить пропущенные элементы в запросах на миграцию, которые были синхронизированы, но не выполнены.</span><span class="sxs-lookup"><span data-stu-id="0c0aa-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="0c0aa-107">$pf = Get – PublicFolderMailboxMigrationRequest | Get – Публикфолдермаилбоксмигратионрекуестстатистикс — IncludeReport; ForEach ($i в $pf) {if ($i. Ларжеитемсенкаунтеред-gt 0-or $i. Бадитемсенкаунтеред-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. Идентифинггуид-Скиппедитемаппровалтиме $ ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="0c0aa-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="0c0aa-108">Пакеты миграции и запросы должны возобновляться и завершаться через несколько минут.</span><span class="sxs-lookup"><span data-stu-id="0c0aa-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

