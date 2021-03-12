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
# <a name="11-call-recording"></a><span data-ttu-id="67a79-102">Запись вызова 1:1</span><span class="sxs-lookup"><span data-stu-id="67a79-102">1:1 call recording</span></span>

<span data-ttu-id="67a79-103">Администраторам необходимо принять меры, чтобы разрешить пользователям записывать вызовы 1:1.</span><span class="sxs-lookup"><span data-stu-id="67a79-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="67a79-104">Начиная с 12 апреля 2021 г. мы начнем применять новый параметр Политики вызовов команд *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="67a79-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="67a79-105">В настоящее время возможности записи вызовов 1:1 контролируются параметром *AllowCloudRecording* в teams Meeting Policies.</span><span class="sxs-lookup"><span data-stu-id="67a79-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="67a79-106">Если пользователям разрешено записывать собрания teams, они также могут записывать вызовы 1:1.</span><span class="sxs-lookup"><span data-stu-id="67a79-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="67a79-107">Если вы предпочитаете блокировать для всех пользователей запись звонков 1:1, вам не нужно принимать никаких действий.</span><span class="sxs-lookup"><span data-stu-id="67a79-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="67a79-108">*Параметр политики вызова AllowCloudRecordingForCalls* будет $False по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="67a79-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="67a79-109">Это изменение задокументировано в следующей публикации Центра сообщений: [(Обновлено) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Введение политики записи вызовов, чтобы задать параметр Teams Calling Policy, который необходимо использовать [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="67a79-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="67a79-110">**Включить запись вызова в 1:1 вызовов:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="67a79-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="67a79-111">Отключение записи вызовов при **звонках 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="67a79-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

