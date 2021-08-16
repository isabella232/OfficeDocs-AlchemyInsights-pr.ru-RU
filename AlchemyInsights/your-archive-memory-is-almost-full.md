---
title: Ваш архивный почтовый ящик почти заполнен
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046765"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Ваш архивный почтовый ящик почти заполнен

Если пользователь получает предупреждение; **Ваш архивный почтовый** ящик почти заполнен, или вам нужно увеличить размер своего архивного почтового ящика, вот несколько советов:

1. Если пользователю назначен Exchange Online План 1, Exchange Online лицензию Plan **2,** чтобы увеличить размер с 50 ГБ до 100 ГБ.
1. Если пользователю уже назначено следующее: **Exchange Online Plan 2** или Exchange Online Plan 1 с надстройка Exchange Online Archiving, используйте ниже шаги, чтобы включить автоматическое расширение архива:.
 
    1. [Подключение Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Запустите следующую командную команду для пользователя:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Запустите следующую команду, чтобы подтвердить, что она включена для пользователя:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Дополнительные сведения см. в следующих разделах.

- [Включить неограниченный архиватив - Справка администратора - Microsoft 365 | Документы Майкрософт](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online ограничения — описание службы | Документы Майкрософт](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Обновление до другого бизнес-плана | Документы Майкрософт](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

