---
title: Включение поддержки размещенной голосовой почты
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608878"
---
# <a name="how-to-enable-hosted-voicemail"></a>Включение поддержки размещенной голосовой почты

Чтобы включить голосовую почту, для **хостедвоицемаил** необходимо задать значение $true.

Свойство **хостедвоицемаил** пользователя, использующего удаленную оболочку POWERSHELL (RPS).

Дополнительные сведения о подключении к RPS приведены в [статье Обзор Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) для получения дополнительных сведений о подключении к RPS.

1. Администратор Teams должен войти в удаленную оболочку PowerShell для Teams.
1. В командной консоли PowerShell администратор Teams может выполнить командлет **Set-csuser user@contoso.com-хостедвоицемаил $true** , в котором находится URI SIP пользователя.

> [!NOTE]
> Репликация изменений в политиках может занять до 24 часов.