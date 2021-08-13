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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966122"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>На портале отсутствуют устройства Configuration Manager

Для синхронизации устройств [обязательные конечные точки в Интернете](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) должны быть доступны на локальном сервере, на котором размещена роль точки подключения службы. Чтобы устранить неполадки с синхронизацией устройств, просмотрите файл **CMGatewaySyncUploadWorker.log**, находящийся в точке подключения службы.

Узнайте больше о том, как [подключить клиент в Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
