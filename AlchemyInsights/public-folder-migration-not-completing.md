---
title: Пакет миграции общедоступных папок не завершается, отображая состояние "Синхронизировано"
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
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406600"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="d50ab-102">Пакет миграции общедоступных папок не завершается, отображая состояние "Синхронизировано"</span><span class="sxs-lookup"><span data-stu-id="d50ab-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="d50ab-103">Вы могли запустить завершение пакета миграции, но пакет миграции продолжает отображать состояние "Синхронизировано" в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="d50ab-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="d50ab-104">Это ожидаемое поведение.</span><span class="sxs-lookup"><span data-stu-id="d50ab-104">This is expected behavior.</span></span>

<span data-ttu-id="d50ab-105">Для пакета миграции нормально оставаться в состоянии "Синхронизировано" в течение нескольких часов, прежде чем переключиться на состояние "Завершение".</span><span class="sxs-lookup"><span data-stu-id="d50ab-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="d50ab-106">Для миграций, включающих большое количество конечных почтовых ящиков, является нормальным сохранение синхронизированного состояния более 24 часов, если не возникало сбоев базовых запросов миграции общедоступных папок и они не помещались на карантин.</span><span class="sxs-lookup"><span data-stu-id="d50ab-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="d50ab-107">Подождите 24–48 часов, пока пакет миграции завершит задачи.</span><span class="sxs-lookup"><span data-stu-id="d50ab-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
