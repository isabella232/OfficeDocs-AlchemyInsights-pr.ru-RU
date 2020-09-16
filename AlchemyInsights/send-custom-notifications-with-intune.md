---
title: Отправка настраиваемых уведомлений с помощью Intune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720659"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Отправка настраиваемых уведомлений пользователям управляемых устройств с iOS и Android

Настраиваемые уведомления для Intune обрабатываются приложением "Корпоративный портал" на устройстве пользователя. Затем приложение создает push-уведомление на этом устройстве.

Ниже перечислены необходимые условия для поддержки получения настраиваемых уведомлений, а также для приложения, которое затем создает push-уведомления.

- На устройстве должно быть установлено приложение "Корпоративный портал".  

- Устройство должно позволять приложению корпоративного портала отправлять push-уведомления. После установки или обновления приложения будет предложено разрешить пользователю отправлять уведомления.

- На устройствах с Android должны быть установлены службы Google проигрывания.

- Устройство должно быть зарегистрировано в Intune.

Дополнительные сведения о том, как отправить сообщение, можно найти в [документации по функциям](https://docs.microsoft.com/intune/custom-notifications).
