---
title: Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве с macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426883"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="13fb4-102">Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве с macOS</span><span class="sxs-lookup"><span data-stu-id="13fb4-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="13fb4-103">Чтобы установить Microsoft Edge в качестве браузера по умолчанию, используйте один из двух способов.</span><span class="sxs-lookup"><span data-stu-id="13fb4-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="13fb4-104">Способ 1. Установите на устройство образ macOS, в котором Microsoft Edge уже установлен в качестве браузера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="13fb4-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="13fb4-105">Способ 2. Установите политику DefaultBrowserSettingEnabled, чтобы пользователю было предложено установить Microsoft Edge в качестве браузера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="13fb4-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="13fb4-106">Любой из этих методов позволяет пользователю изменить браузер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="13fb4-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="13fb4-107">По этой причине мы рекомендуем развернуть политику DefaultBrowserSettingEnabled, даже если вы использовали способ 1.</span><span class="sxs-lookup"><span data-stu-id="13fb4-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="13fb4-108">Если пользователь изменяет браузер по умолчанию после развертывания политики, пользователю будет предложено вернуть Microsoft Edge в качестве браузера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="13fb4-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
