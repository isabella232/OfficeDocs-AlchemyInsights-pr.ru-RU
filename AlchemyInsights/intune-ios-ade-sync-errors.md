---
title: Ошибки синхронизации автоматической регистрации устройств Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707891"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="4cac1-102">Ошибки синхронизации автоматической регистрации устройств Apple</span><span class="sxs-lookup"><span data-stu-id="4cac1-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="4cac1-103">"Мы обнаружили, что у вас есть один или несколько маркеров ADE/DEP, которые находятся в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="4cac1-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="4cac1-104">Пока состояние ошибки не будет устранено для каждого затронутого маркера, функция ADE не будет работать для одного и того же".</span><span class="sxs-lookup"><span data-stu-id="4cac1-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="4cac1-105">Эта ошибка может возникнуть по ряду способов, в том числе:</span><span class="sxs-lookup"><span data-stu-id="4cac1-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="4cac1-106">Устройства могут не синхронизироваться с Intune с ABM/ASM</span><span class="sxs-lookup"><span data-stu-id="4cac1-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="4cac1-107">Сбой назначений профиля регистрации</span><span class="sxs-lookup"><span data-stu-id="4cac1-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="4cac1-108">Устройства могут не пройти регистрацию в ADE успешно</span><span class="sxs-lookup"><span data-stu-id="4cac1-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="4cac1-109">Проверьте ошибку синхронизации, зарегистрированную в консоли Intune в подсети "Устройства > Регистрация устройств > маркеры программы регистрации **Apple >"** и просмотрите следующую документацию, чтобы просмотреть возможные исправление:</span><span class="sxs-lookup"><span data-stu-id="4cac1-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="4cac1-110">Ошибки синхронизации ABM/ASM для маркеров автоматической регистрации устройств iOS, iPadOS и macOS</span><span class="sxs-lookup"><span data-stu-id="4cac1-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
