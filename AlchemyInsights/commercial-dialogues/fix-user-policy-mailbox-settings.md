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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034731"
---
# <a name="fix-user-policymailbox-settings"></a>Исправление параметров политики пользователя и почтовых ящиков

Параметры нежелательной почты в почтовом ящике повлияли на это сообщение. Чтобы просмотреть параметры, сделайте следующее:

1. Запуск Exchange управленческой оболочки. Дополнительные сведения см. в [Exchange Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Запустите эту команду (используя адрес электронной почты  **пользователя): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Проверьте, является ли адрес электронной почты отправителей частью **TrustedSendersAndDomains** или **BlockedSendersAndDomains.** Если адрес электронной почты находится в одном из списков, его может потребоваться удалить. Дополнительные дополнительные сообщения см. [в сообщении Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
