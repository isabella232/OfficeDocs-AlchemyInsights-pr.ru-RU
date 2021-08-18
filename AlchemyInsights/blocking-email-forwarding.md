---
title: Блокировать или разблокировать внешнюю автоматическую переадружение электронной почты
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315887"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Блокировать или разблокировать вечную автоматическую переададку электронной почты

Чтобы включить или отключить пересылку электронной почты для определенного почтового ящика, см. [в сообщении Configure email forwarding.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Администраторы могут управлять внешними переададантами для организации с помощью [исходящие политики нежелательной почты.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Вы управляете исходящей политикой нежелательной почты на портале Microsoft 365 Defender на портале <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) в Exchange Online PowerShell.

Если вы получаете следующую ошибку: "Отказано в доступе **550 5.7.520,** ваша организация не разрешает внешнюю переадрешение", убедитесь, что политика настроена, чтобы включить внешние автоматические сообщения.

**Примечание.** Мы рекомендовали значение по умолчанию Automatic **- System controlled** for the **Automatic forwarding rules** setting in your default outbound spam filter policy (automatic external forwarding is blocked; internal automatic forwarding still works). Необходимо создать настраиваемые политики фильтрации исходящие нежелательной почты и использовать значение **On - Переадружение** включено только для пользователей, которым требуется внешняя автоматическая переадружение электронной почты. Дополнительные сведения см. в [сообщении Configuring external email forwarding in Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
