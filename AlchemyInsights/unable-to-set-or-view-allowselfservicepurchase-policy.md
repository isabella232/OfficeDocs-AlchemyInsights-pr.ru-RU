---
title: Невозможно установить или просмотреть политику AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020205"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Невозможно установить или просмотреть политику AllowSelfServicePurchase

При попытке настроить или просмотреть политику AllowSelfServicePurchase вы получите следующее сообщение об ошибке:

*HandleError. Не удалось получить политику продукта с помощью PolicyId 'AllowSelfServicePurchase', ErrorMessage . При отправке было закрыто первое подключение. При отправке произошла неожиданная ошибка.*

Это может быть связано со старой версией безопасности транспортного слоя (TLS). Чтобы подключить службу MSCommerce, необходимо использовать TLS 1.2 или более.  

Попробуйте следующие действия, чтобы включить и установить протокол TLS до 1.2, проверить и повторить.
 1. В командной подсказке PowerShell (PS C: введите следующую команду, чтобы установить протокол TLS версии \) 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Убедитесь в использовании протокола TLS со следующей командой:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Повторное просмотр команд Get или Update по мере необходимости.

