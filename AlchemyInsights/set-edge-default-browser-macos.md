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
ms.openlocfilehash: e04f8931ef12c426a5c3d5f617fc5f5d5c3a15c6fe43f7b84a7e97e8ee04e3fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073973"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве с macOS

Чтобы установить Microsoft Edge в качестве браузера по умолчанию, используйте один из двух способов.

Способ 1. Установите на устройство образ macOS, в котором Microsoft Edge уже установлен в качестве браузера по умолчанию.

Способ 2. Установите политику DefaultBrowserSettingEnabled, чтобы пользователю было предложено установить Microsoft Edge в качестве браузера по умолчанию.

Любой из этих методов позволяет пользователю изменить браузер по умолчанию. По этой причине мы рекомендуем развернуть политику DefaultBrowserSettingEnabled, даже если вы использовали способ 1. Если пользователь изменяет браузер по умолчанию после развертывания политики, пользователю будет предложено вернуть Microsoft Edge в качестве браузера по умолчанию.
