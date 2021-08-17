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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314397"
---
# <a name="11-call-recording"></a>Запись вызова 1:1

Если **в** вызове 1:1 кнопка "Начните запись" сеет, необходимо изменить параметры политики для пользователя, находящегося под влиянием. Чтобы проверить параметр политики, запустите диагностику для пользователя, набрав **diag: Teams 1:1 Запись вызовов** выше.     

Начиная с 31 мая 2021 г. мы начнем применять новую политику вызовов Teams *AllowCloudRecordingForCalls*. До этого изменения запись вызовов 1:1 контролируется политикой *собрания AllowCloudRecording* Teams. Это изменение задокументировано в сообщении Центра сообщений: [(Обновлено) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Введение политики записи вызовов .  

*AllowCloudRecordingForCalls*   Параметр политики вызовов установлен **для** $False по умолчанию. Если вы предпочитаете блокировать для всех пользователей запись звонков 1:1, вам не нужно принимать никаких действий.  

Чтобы включить запись вызовов для всех пользователей в 1:1, [используйте Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) для запуска следующего cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Кроме того, можно создать новую политику и задать **-AllowCloudRecordingForCalls** для $true и назначить эту политику пользователям.  

Дополнительные сведения см. в 1:1 Элемент управления политиками записи [вызовов : (Почти!) Здесь](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
