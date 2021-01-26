---
title: Архивный почтовый ящик почти заполнен
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950515"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Архивный почтовый ящик почти заполнен

Если пользователь получает предупреждение; **Архивный почтовый ящик** почти заполнен, или вам нужно увеличить размер архивного почтового ящика, вот несколько советов:

1. Если пользователю назначена лицензия Exchange Online (план 1), обновим лицензию на **Exchange Online (план 2),** чтобы увеличить размер с 50 ГБ до 100 ГБ.
1. Если пользователю уже назначена любая из следующих надстроек: **Exchange Online (план 2)** или Exchange Online (план 1) с надстройка архивация на базе Exchange Online, воспользуйтесь следующими действиями для автоматического расширения архивов.
 
    1. [Подключись к Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Запустите следующий командлет для пользователя:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Чтобы подтвердить, что он включен для пользователя, запустите следующий командлет:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Дополнительные сведения см. в указанных ниже статьях.    

- [ Включить неограниченный архив — справка для администраторов - Соответствие требованиям Microsoft 365 | Документы Майкрософт](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Ограничения Exchange Online — описание службы | Документы Майкрософт](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Обновление до другой бизнес-| Документы Майкрософт](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

