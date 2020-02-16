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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Для пакета миграции общедоступных папок с состоянием Комплетедвисеррорс

Выполните следующие действия, чтобы завершить пакет, пропуская крупные или поврежденные элементы: 
1. Утвердите пропущенные элементы в пакете миграции:

    Set — MigrationBatch \<BatchName> аппровескиппедитемс 
2. Используйте следующую команду, чтобы утвердить пропущенные элементы в запросах на миграцию, которые были синхронизированы, но не выполнены.

    $pf = Get – PublicFolderMailboxMigrationRequest | Get – Публикфолдермаилбоксмигратионрекуестстатистикс — IncludeReport; ForEach ($i в $pf) {if ($i. Ларжеитемсенкаунтеред-gt 0-or $i. Бадитемсенкаунтеред-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. Идентифинггуид-Скиппедитемаппровалтиме $ ([DateTime]:: UtcNow)}}
3. Пакеты миграции и запросы должны возобновляться и завершаться через несколько минут.

