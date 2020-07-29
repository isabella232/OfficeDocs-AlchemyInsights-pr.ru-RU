---
title: Сброс ПИН-кода или пароля устройства из Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431677"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="de030-102">Сброс ПИН-кода или пароля устройства из Intune</span><span class="sxs-lookup"><span data-stu-id="de030-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="de030-103">Вы можете удалить секретный код или заставить пользователя создать новый секретный код в Intune для устройства с iOS или Android, воспользовавшись действием удаления секретного кода.</span><span class="sxs-lookup"><span data-stu-id="de030-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="de030-104">Это действие поддерживают только определенные типы операционных систем и типы рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="de030-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="de030-105">Дополнительные сведения о поддерживаемых платформах и запуске сброса секретного кода см. в статье [Сброс и удаление секретного кода устройства в Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span><span class="sxs-lookup"><span data-stu-id="de030-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="de030-106">Вы можете сбросить существующий ПИН-код до нового значения, используя действие сброса ПИН-кода на устройствах с операционной системой Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="de030-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="de030-107">Это позволит пользователю разблокировать устройство и настроить новый ПИН-код.</span><span class="sxs-lookup"><span data-stu-id="de030-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="de030-108">Дополнительные сведения см. в статье [Сброс секретного кода на устройствах с Windows с помощью Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span><span class="sxs-lookup"><span data-stu-id="de030-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>