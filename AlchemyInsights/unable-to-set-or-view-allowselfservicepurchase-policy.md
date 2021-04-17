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
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826104"
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

