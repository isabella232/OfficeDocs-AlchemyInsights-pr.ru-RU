---
title: Запись вызова 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733862"
---
# <a name="11-call-recording"></a>Запись вызова 1:1

Администраторам необходимо принять меры, чтобы разрешить пользователям записывать вызовы 1:1.
 
Начиная с 12 апреля 2021 г. мы начнем применять новый параметр Политики вызовов команд *AllowCloudRecordingForCalls.* 

В настоящее время возможности записи вызовов 1:1 контролируются параметром *AllowCloudRecording* в teams Meeting Policies. Если пользователям разрешено записывать собрания teams, они также могут записывать вызовы 1:1.

Если вы предпочитаете блокировать для всех пользователей запись звонков 1:1, вам не нужно принимать никаких действий. *Параметр политики вызова AllowCloudRecordingForCalls* будет $False по умолчанию.

Это изменение задокументировано в следующей публикации Центра сообщений: [(Обновлено) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Введение политики записи вызовов, чтобы задать параметр Teams Calling Policy, который необходимо использовать [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Включить запись вызова в 1:1 вызовов:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

Отключение записи вызовов при **звонках 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

