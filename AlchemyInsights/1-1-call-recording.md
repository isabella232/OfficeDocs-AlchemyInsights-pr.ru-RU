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
ms.openlocfilehash: befb89c28396be3dc60d9d812a0c6aced69bea3c1c48d88a4ab81a34d6c259b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919004"
---
# <a name="11-call-recording"></a>Запись вызова 1:1

Если **в** вызове 1:1 кнопка "Начните запись" сеет, необходимо изменить параметры политики для пользователя, находящегося под влиянием. Чтобы проверить параметр политики, запустите диагностику для пользователя, набрав **diag: Teams 1:1 Запись вызовов** выше.     

Начиная с 31 мая 2021 г. мы начнем применять новую политику вызовов Teams *AllowCloudRecordingForCalls*. До этого изменения запись вызовов 1:1 контролируется политикой *собрания AllowCloudRecording* Teams. Это изменение задокументировано в сообщении Центра сообщений: [(Обновлено) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Введение политики записи вызовов .  

*AllowCloudRecordingForCalls*   Параметр политики вызовов установлен **для** $False по умолчанию. Если вы предпочитаете блокировать для всех пользователей запись звонков 1:1, вам не нужно принимать никаких действий.  

Чтобы включить запись вызовов для всех пользователей в 1:1, [используйте Teams PowerShell](/microsoftteams/teams-powershell-install) для запуска следующего cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Кроме того, можно создать новую политику и задать **-AllowCloudRecordingForCalls** для $true и назначить эту политику пользователям.  

Дополнительные сведения см. в 1:1 Элемент управления политиками записи [вызовов : (Почти!) Здесь](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
