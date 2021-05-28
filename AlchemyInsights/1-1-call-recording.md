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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696971"
---
# <a name="11-call-recording"></a><span data-ttu-id="0a0da-102">Запись вызова 1:1</span><span class="sxs-lookup"><span data-stu-id="0a0da-102">1:1 call recording</span></span>

<span data-ttu-id="0a0da-103">Если **в** вызове 1:1 кнопка "Начните запись" сеет, необходимо изменить параметры политики для пользователя, находящегося под влиянием.</span><span class="sxs-lookup"><span data-stu-id="0a0da-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="0a0da-104">Начиная с 31 мая 2021 г. мы начнем применять новую политику вызовов Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="0a0da-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="0a0da-105">До этого изменения запись вызовов 1:1 контролируется политикой *собрания AllowCloudRecording* Teams.</span><span class="sxs-lookup"><span data-stu-id="0a0da-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="0a0da-106">Это изменение задокументировано в сообщении Центра сообщений: [(Обновлено) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Введение политики записи вызовов .</span><span class="sxs-lookup"><span data-stu-id="0a0da-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="0a0da-107">*AllowCloudRecordingForCalls*   Параметр политики вызовов установлен **для** $False по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0a0da-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="0a0da-108">Если вы предпочитаете блокировать для всех пользователей запись звонков 1:1, вам не нужно принимать никаких действий.</span><span class="sxs-lookup"><span data-stu-id="0a0da-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="0a0da-109">Чтобы включить запись вызовов для всех пользователей в 1:1, используйте Teams PowerShell для запуска следующего cmdlet:</span><span class="sxs-lookup"><span data-stu-id="0a0da-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="0a0da-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="0a0da-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="0a0da-111">Кроме того, можно создать новую политику и задать **-AllowCloudRecordingForCalls** для $true и назначить эту политику пользователям. </span><span class="sxs-lookup"><span data-stu-id="0a0da-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="0a0da-112">Дополнительные сведения см. в 1:1 Элемент управления политиками записи [вызовов : (Почти!) Здесь](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="0a0da-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
