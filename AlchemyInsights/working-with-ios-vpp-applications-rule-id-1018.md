---
title: Работа с ID 1018 приложениями VPP iOS
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083027"
---
# <a name="working-with-ios-vpp-applications"></a>Работа с приложениями VPP для iOS

Узнайте, как управлять приложениями [для iOS,](https://docs.microsoft.com/intune/vpp-apps-ios) приобретенными с помощью программы покупки тома с помощью Microsoft Intune, чтобы узнать о свойствах, ограничениях и шагах по использованию программы покупки томов Apple и ее поддержке в Microsoft Intune.
  
 **Общие проблемы:** "Я направил пользователям приложение VPP для iOS, но установка не удалась".
  
- Это может произойти, если один маркер VPP используется для нескольких поставщиков управления мобильными устройствами. Маркеры VPP от Apple можно использовать только с одним поставщиком. Если вы использовали маркер VPP с несколькими поставщиками, необходимо повторно загрузить его в Intune.

- Установка также может привести к сбойу, если общее число установок превышает количество лицензий. Чтобы просмотреть отчет об использовании лицензий, перейдите на страницу **Лицензии приложений для мобильных приложений Intune.** \>  Подробнее о восстановлении лицензий в использовании [см. в этой статье.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
