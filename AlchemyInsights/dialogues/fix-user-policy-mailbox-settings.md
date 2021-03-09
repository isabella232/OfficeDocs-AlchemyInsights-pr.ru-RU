---
title: Исправление параметров политики пользователя и почтовых ящиков
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568687"
---
# <a name="fix-user-policymailbox-settings"></a>Исправление параметров политики пользователя и почтовых ящиков

Параметры нежелательной почты в почтовом ящике повлияли на это сообщение. Чтобы просмотреть параметры, сделайте следующее:

1. Запуск оболочки управления Exchange. Дополнительные сведения см. в [рублях Open the Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Запустите эту команду (используя адрес электронной почты  **пользователя): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Проверьте, является ли адрес электронной почты отправителей частью **TrustedSendersAndDomains** или **BlockedSendersAndDomains.** Если адрес электронной почты находится в одном из списков, его может потребоваться удалить. Дополнительные дополнительные сообщения см. [в сообщении Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
