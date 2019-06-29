---
title: Работа с идентификатором правила приложений для iOS VPP 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364877"
---
# <a name="working-with-ios-vpp-applications"></a>Работа с приложениями для iOS VPP

Узнайте, [как управлять приложениями для iOS, приобретенными через программу Volume-Purchase, с помощью Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , чтобы узнать о возможностях, ограничениях и действиях по использованию программы Apple Volume Purchase Program, а также ее поддержке в Microsoft Intune.
  
 **Распространенные проблемы:** "Мне назначено приложение для iOS VPP для пользователей, но не удалось выполнить установку".
  
- Это может произойти, если один токен VPP используется для нескольких поставщиков услуг управления мобильными устройствами. Токены VPP от Apple можно использовать только с одним поставщиком. Если вы использовали токен VPP с несколькими поставщиками, необходимо повторно отправить маркер в Intune.

- Установка также может быть неисправной, если общее число установок превышает количество лицензий. Чтобы просмотреть отчет об использовании лицензий, перейдите на страницу " \> **лицензии приложения** для **мобильных приложений Intune** ". Сведения о том, как повторно использовать лицензии, можно найти в [этой статье.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
