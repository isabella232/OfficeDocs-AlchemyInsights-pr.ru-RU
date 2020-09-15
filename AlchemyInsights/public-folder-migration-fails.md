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
# <a name="public-folder-migration-fails-at-95"></a>Сбой миграции общедоступной папки на уровне 95 %

Вы могли запустить завершение пакета миграции, но пакет миграции продолжает отображать состояние **Синхронизировано** в течение длительного времени. Это ожидаемое поведение.

Для пакета миграции нормально оставаться в состоянии **Синхронизировано** в течение нескольких часов, прежде чем переключиться на состояние **Завершение**. Для миграций, включающих большое количество конечных почтовых ящиков, является нормальным сохранение синхронизированного состояния более 24 часов, если не возникало сбоев базовых запросов миграции общедоступных папок и они не помещались на карантин. Подождите 24–48 часов, пока пакет миграции завершит задачи.

При сбое миграции общедоступных папок на уровне 95% с ошибкой FailedToMailEnablePublicFoldersException:

1. Скачайте и запустите сценарий [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) на локальном сервере Exchange.

2. Выполните действия по исправлению, предлагаемые сценарием.

3. Выполните команду Sync-MailPublicFolders (для Exchange 2010) или Sync-ModernMailPublicFolders (для Exchange 2013 и более поздних версий).

4. Возобновите миграцию общедоступной папки.
