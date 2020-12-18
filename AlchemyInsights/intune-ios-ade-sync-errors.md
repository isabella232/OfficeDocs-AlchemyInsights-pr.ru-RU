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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Ошибки синхронизации автоматической регистрации устройств Apple

"Мы обнаружили, что у вас есть один или несколько маркеров ADE/DEP, которые находятся в состоянии ошибки. Пока состояние ошибки не будет устранено для каждого затронутого маркера, функция ADE не будет работать для одного и того же".

Эта ошибка может возникнуть по ряду способов, в том числе:

1. Устройства могут не синхронизироваться с Intune с ABM/ASM
2. Сбой назначений профиля регистрации
3. Устройства могут не пройти регистрацию в ADE успешно

Проверьте ошибку синхронизации, зарегистрированную в консоли Intune в подсети "Устройства > Регистрация устройств > маркеры программы регистрации **Apple >"** и просмотрите следующую документацию, чтобы просмотреть возможные исправление:

[Ошибки синхронизации ABM/ASM для маркеров автоматической регистрации устройств iOS, iPadOS и macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
