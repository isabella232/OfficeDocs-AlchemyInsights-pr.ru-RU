---
title: Не удается задать или просмотреть политику Алловселфсервицепурчасе
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158574"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не удается задать или просмотреть политику Алловселфсервицепурчасе

При попытке задать или просмотреть политику Алловселфсервицепурчасе появляется следующее сообщение об ошибке:

*HandleError: не удалось получить политику продукта с Полициид "Алловселфсервицепурчасе", ErrorMessage — базовое подключение было закрыто: при отправке произошла непредвиденная ошибка.*

Это может быть вызвано более старой версией протокола TLS. Чтобы подключить службу Мскоммерце, необходимо использовать протокол TLS 1,2 или более поздней версии.  

Выполните следующие действия, чтобы включить или отключить протокол TLS равным 1,2, проверить и повторить попытку.
 1. В командной командной консоли PowerShell (PS C:\) введите следующую команду, чтобы установить для протокола TLS версии 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Проверьте использование протоколов TLS с помощью следующей команды:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Повторите команды Get или Update по мере необходимости.

