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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013761"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Ошибки синхронизации синхронизации автоматического устройства Apple

"Мы обнаружили, что у вас есть один или несколько маркеров ADE/DEP, которые находятся в состоянии ошибки. Пока состояние ошибки не будет разрешено для каждого затронутого маркера, функциональность ADE будет работать не так, как ожидалось".

Эта ошибка может проявляться по ряду способов, включая:

1. Устройства не могут синхронизироваться с ABM/ASM на Intune
2. Назначения профилей регистрации могут быть сбоями
3. Устройства могут не успешно завершить регистрацию ADE

Проверьте, есть ли ошибка синхронизации, зарегистрированная в консоли Intune в консоли Devices > Enroll Devices > токенов программы > **регистрации.**

Одной из наиболее распространенных причин ошибки синхронизации является истечение срока действия текущего маркера. Во многих случаях обновление затронутого маркера позволит устранить проблему.

Если срок действия одного или более маркеров истек, см. в следующей документации, которая поможет вам обновить их по мере необходимости:

[Обновление маркера автоматической регистрации устройств](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Кроме того, вы можете увидеть следующую документацию, чтобы увидеть возможные устранения других ошибок, вызывающих сбои синхронизации маркеров:

[Ошибки синхронизации ABM/ASM для маркеров автоматической регистрации устройств iOS/iPadOS и macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Ошибки синхронизации ABM/ASM для маркеров автоматической регистрации устройств iOS/iPadOS и macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
