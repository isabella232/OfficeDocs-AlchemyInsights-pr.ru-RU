---
title: На портале отсутствуют устройства Configuration Manager
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817257"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>На портале отсутствуют устройства Configuration Manager

Для синхронизации устройств [обязательные конечные точки в Интернете](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) должны быть доступны на локальном сервере, на котором размещена роль точки подключения службы. Чтобы устранить неполадки с синхронизацией устройств, просмотрите файл **CMGatewaySyncUploadWorker.log**, находящийся в точке подключения службы.

Узнайте больше о том, как [подключить клиент в Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
