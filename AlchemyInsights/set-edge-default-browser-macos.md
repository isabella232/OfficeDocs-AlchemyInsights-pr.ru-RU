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
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве с macOS

Чтобы установить Microsoft Edge в качестве браузера по умолчанию, используйте один из двух способов.

Способ 1. Установите на устройство образ macOS, в котором Microsoft Edge уже установлен в качестве браузера по умолчанию.

Способ 2. Установите политику DefaultBrowserSettingEnabled, чтобы пользователю было предложено установить Microsoft Edge в качестве браузера по умолчанию.

Любой из этих методов позволяет пользователю изменить браузер по умолчанию. По этой причине мы рекомендуем развернуть политику DefaultBrowserSettingEnabled, даже если вы использовали способ 1. Если пользователь изменяет браузер по умолчанию после развертывания политики, пользователю будет предложено вернуть Microsoft Edge в качестве браузера по умолчанию.
