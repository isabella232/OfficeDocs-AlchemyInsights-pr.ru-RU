---
title: На портале отсутствуют устройства Configuration Manager
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790230"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>На портале отсутствуют устройства Configuration Manager

Для синхронизации устройств [обязательные конечные точки в Интернете](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) должны быть доступны на локальном сервере, на котором размещена роль точки подключения службы. Чтобы устранить неполадки с синхронизацией устройств, просмотрите файл **CMGatewaySyncUploadWorker.log**, находящийся в точке подключения службы.

Узнайте больше о том, как [подключить клиент в Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
