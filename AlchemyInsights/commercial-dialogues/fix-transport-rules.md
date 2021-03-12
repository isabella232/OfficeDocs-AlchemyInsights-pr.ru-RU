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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737825"
---
# <a name="fix-transport-rules"></a>Исправление правил транспорта

На это сообщение повлияло правило пользовательского потока почты. Чтобы просмотреть точное правило, сделайте следующее:

1. В результатах отправки в **статье Дополнительные сведения** обратите внимание на **GUID** или **имя политики.**
2. Запуск оболочки управления Exchange. Дополнительные сведения см. в [рублях Open the Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Запустите эту команду (с помощью GUID из отправки): **Get-TransportRule -identity "GUID"** | fl * Description*
4. Просмотрите описание, чтобы просмотреть настроенные условия, которые повлияли на сообщение.

Дополнительные дополнительные информации [см. в см. в ленте Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
