---
title: Ошибки синхронизации синхронизации автоматического устройства Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448935"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="91d02-102">Ошибки синхронизации синхронизации автоматического устройства Apple</span><span class="sxs-lookup"><span data-stu-id="91d02-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="91d02-103">"Мы обнаружили, что у вас есть один или несколько маркеров ADE/DEP, которые находятся в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="91d02-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="91d02-104">Пока состояние ошибки не будет разрешено для каждого затронутого маркера, функциональность ADE будет работать не так, как ожидалось".</span><span class="sxs-lookup"><span data-stu-id="91d02-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="91d02-105">Эта ошибка может проявляться по ряду способов, включая:</span><span class="sxs-lookup"><span data-stu-id="91d02-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="91d02-106">Устройства не могут синхронизироваться с ABM/ASM на Intune</span><span class="sxs-lookup"><span data-stu-id="91d02-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="91d02-107">Назначения профилей регистрации могут быть сбоями</span><span class="sxs-lookup"><span data-stu-id="91d02-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="91d02-108">Устройства могут не успешно завершить регистрацию ADE</span><span class="sxs-lookup"><span data-stu-id="91d02-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="91d02-109">Проверьте, есть ли ошибка синхронизации, зарегистрированная в консоли Intune в консоли Devices > Enroll Devices > токенов программы > **регистрации.**</span><span class="sxs-lookup"><span data-stu-id="91d02-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="91d02-110">Одной из наиболее распространенных причин ошибки синхронизации является истечение срока действия текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="91d02-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="91d02-111">Во многих случаях обновление затронутого маркера позволит устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="91d02-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="91d02-112">Если срок действия одного или более маркеров истек, см. в следующей документации, которая поможет вам обновить их по мере необходимости:</span><span class="sxs-lookup"><span data-stu-id="91d02-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="91d02-113">Обновление маркера автоматической регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="91d02-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="91d02-114">Кроме того, вы можете увидеть следующую документацию, чтобы увидеть возможные устранения других ошибок, вызывающих сбои синхронизации маркеров:</span><span class="sxs-lookup"><span data-stu-id="91d02-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="91d02-115">Ошибки синхронизации ABM/ASM для маркеров автоматической регистрации устройств iOS/iPadOS и macOS</span><span class="sxs-lookup"><span data-stu-id="91d02-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="91d02-116">Ошибки синхронизации ABM/ASM для маркеров автоматической регистрации устройств iOS/iPadOS и macOS</span><span class="sxs-lookup"><span data-stu-id="91d02-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
