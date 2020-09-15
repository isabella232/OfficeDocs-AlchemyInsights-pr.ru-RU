---
title: Сбой миграции общедоступной папки на уровне 95 %
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662425"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="2dd30-102">Сбой миграции общедоступной папки на уровне 95 %</span><span class="sxs-lookup"><span data-stu-id="2dd30-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="2dd30-103">Вы могли запустить завершение пакета миграции, но пакет миграции продолжает отображать состояние **Синхронизировано** в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="2dd30-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="2dd30-104">Это ожидаемое поведение.</span><span class="sxs-lookup"><span data-stu-id="2dd30-104">This is expected behavior.</span></span>

<span data-ttu-id="2dd30-105">Для пакета миграции нормально оставаться в состоянии **Синхронизировано** в течение нескольких часов, прежде чем переключиться на состояние **Завершение**.</span><span class="sxs-lookup"><span data-stu-id="2dd30-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="2dd30-106">Для миграций, включающих большое количество конечных почтовых ящиков, является нормальным сохранение синхронизированного состояния более 24 часов, если не возникало сбоев базовых запросов миграции общедоступных папок и они не помещались на карантин.</span><span class="sxs-lookup"><span data-stu-id="2dd30-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="2dd30-107">Подождите 24–48 часов, пока пакет миграции завершит задачи.</span><span class="sxs-lookup"><span data-stu-id="2dd30-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="2dd30-108">При сбое миграции общедоступных папок на уровне 95% с ошибкой FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="2dd30-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="2dd30-109">Скачайте и запустите сценарий [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) на локальном сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dd30-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="2dd30-110">Выполните действия по исправлению, предлагаемые сценарием.</span><span class="sxs-lookup"><span data-stu-id="2dd30-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="2dd30-111">Выполните команду Sync-MailPublicFolders (для Exchange 2010) или Sync-ModernMailPublicFolders (для Exchange 2013 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="2dd30-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="2dd30-112">Возобновите миграцию общедоступной папки.</span><span class="sxs-lookup"><span data-stu-id="2dd30-112">Resume public folder migration.</span></span>
