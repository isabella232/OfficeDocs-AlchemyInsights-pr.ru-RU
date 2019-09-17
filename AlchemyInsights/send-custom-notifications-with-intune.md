---
title: Отправка настраиваемых уведомлений с помощью Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992325"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Отправка настраиваемых уведомлений пользователям управляемых устройств с iOS и Android

Настраиваемые уведомления для Intune обрабатываются приложением "Корпоративный портал" на устройстве пользователя. Затем приложение создает push-уведомление на этом устройстве.

Ниже перечислены необходимые условия для поддержки получения настраиваемых уведомлений, а также для приложения, которое затем создает push-уведомления.

- На устройстве должно быть установлено приложение "Корпоративный портал".  

- Устройство должно позволять приложению корпоративного портала отправлять push-уведомления. После установки или обновления приложения будет предложено разрешить пользователю отправлять уведомления.

- На устройствах с Android должны быть установлены службы Google проигрывания.

- Устройство должно быть зарегистрировано в Intune.

Дополнительные сведения о том, как отправить сообщение, можно найти в [документации по функциям](https://docs.microsoft.com/intune/custom-notifications).
