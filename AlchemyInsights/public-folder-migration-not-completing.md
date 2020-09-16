---
title: Пакет миграции общедоступных папок не завершается, отображая состояние "Синхронизировано"
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
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771490"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="29595-102">Пакет миграции общедоступных папок не завершается, отображая состояние "Синхронизировано"</span><span class="sxs-lookup"><span data-stu-id="29595-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="29595-103">Вы могли запустить завершение пакета миграции, но пакет миграции продолжает отображать состояние "Синхронизировано" в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="29595-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="29595-104">Это ожидаемое поведение.</span><span class="sxs-lookup"><span data-stu-id="29595-104">This is expected behavior.</span></span>

<span data-ttu-id="29595-105">Для пакета миграции нормально оставаться в состоянии "Синхронизировано" в течение нескольких часов, прежде чем переключиться на состояние "Завершение".</span><span class="sxs-lookup"><span data-stu-id="29595-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="29595-106">Для миграций, включающих большое количество конечных почтовых ящиков, является нормальным сохранение синхронизированного состояния более 24 часов, если не возникало сбоев базовых запросов миграции общедоступных папок и они не помещались на карантин.</span><span class="sxs-lookup"><span data-stu-id="29595-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="29595-107">Подождите 24–48 часов, пока пакет миграции завершит задачи.</span><span class="sxs-lookup"><span data-stu-id="29595-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
