---
title: Как включить хозяйную голосовую почту
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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055567"
---
# <a name="how-to-enable-hosted-voicemail"></a>Как включить хозяйную голосовую почту

Чтобы включить голосовую почту, **hostedVoicemail** должна быть настроена $true.

Свойство **HostedVoicemail** для пользователя с помощью удаленной powerShell (RPS).

Дополнительные сведения о подключении к RPS см. в Microsoft Teams [Обзор PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)

1. Администратор Teams войти в удаленную powerShell для Teams.
1. Из PowerShell подсказок Teams администратор может запускать **set-csuser user@contoso.com-HostedVoiceMail $true** где sip uri является пользователем, о котором идет речь.

> [!NOTE]
> Репликация изменений политик может занять до 24 часов.