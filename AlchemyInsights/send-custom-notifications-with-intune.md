---
title: Отправка пользовательских уведомлений с помощью Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086177"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Отправка пользовательских уведомлений пользователям управляемых устройств с iOS и Android

Настраиваемые уведомления для Intune обрабатываются приложением Корпоративный портал на устройстве пользователя. Затем приложение создает push-уведомление на этом устройстве.

Ниже приводится условие устройства для поддержки получения пользовательских уведомлений, а также создание приложения push-уведомления.

- На устройстве должно быть Корпоративный портал приложение.  

- Устройство должно разрешить приложению Корпоративный портал отправку push-уведомлений. При установке или обновлении приложения пользователю будет предложено разрешить уведомления.

- На устройствах Android должны быть установлены службы Google Play.

- Устройство должно быть зарегистрироваться с помощью Intune.

Дополнительные сведения, включая отправку сообщения, см. в [документации по функции.](https://docs.microsoft.com/intune/custom-notifications)
