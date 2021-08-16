---
title: Исправление правил транспорта
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034767"
---
# <a name="fix-transport-rules"></a>Исправление правил транспорта

На это сообщение повлияло правило пользовательского потока почты. Чтобы просмотреть точное правило, сделайте следующее:

1. В результатах отправки в **статье Дополнительные сведения** обратите внимание на **GUID** или **имя политики.**
2. Запуск Exchange управленческой оболочки. Дополнительные сведения см. в [Exchange Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Запустите эту команду (с помощью GUID из отправки): **Get-TransportRule -identity "GUID"** | fl * Description*
4. Просмотрите описание, чтобы просмотреть настроенные условия, которые повлияли на сообщение.

Дополнительные дополнительные информации [см. в см. в ленте Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
