---
title: Использование диспетчера конфигураций для развертывания, обновления и управления Microsoft EDGE в Windows
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004030"
- "7100"
ms.openlocfilehash: ee978146ff0964e9ebd9f476f9c92d1f97aa042c
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600141"
---
# <a name="use-configuration-manager-to-deploy-update-and-manage-microsoft-edge-on-windows"></a><span data-ttu-id="8511a-102">Использование диспетчера конфигураций для развертывания, обновления и управления Microsoft EDGE в Windows</span><span class="sxs-lookup"><span data-stu-id="8511a-102">Use Configuration Manager to deploy, update, and manage Microsoft Edge on Windows</span></span>

<span data-ttu-id="8511a-103">По мере использования Configuration Manager версии 1910 можно развернуть Microsoft EDGE (версии 77 и более поздней версии) с помощью скрипта PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8511a-103">As of Configuration Manager version 1910, you can deploy Microsoft Edge (versions 77 and later) through a PowerShell script.</span></span> <span data-ttu-id="8511a-104">В сценарии отключается автоматическое обновление, и это позволяет управлять обновлениями с помощью Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8511a-104">The script turns off automatic updates, and this lets you manage the updates through Configuration Manager.</span></span> <span data-ttu-id="8511a-105">Чтобы узнать больше об этом и других преимуществах использования диспетчера конфигураций, ознакомьтесь со статьей [Microsoft Edge Management](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge?).</span><span class="sxs-lookup"><span data-stu-id="8511a-105">To learn more about this and other benefits of using Configuration Manager, see [Microsoft Edge Management](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge?).</span></span>