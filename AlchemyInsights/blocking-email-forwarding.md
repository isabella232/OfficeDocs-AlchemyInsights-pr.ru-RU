---
title: 726 Блокировка отправки электронной почты
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059645"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Блокировка или разблокировка переададровки электронной почты

Чтобы включить или отключить пересылку электронной почты для определенного почтового ящика, см. [в сообщении Configure email forwarding.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

На уровне клиента управление внешней переададантной рассылкой происходит с помощью политики исходящие нежелательной почты. Вы можете проверить политику исходящего фильтра [](https://protection.office.com/antispam) нежелательной почты из Центра безопасности и соответствия требованиям здесь или с помощью команды [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Если вы получаете следующую ошибку: "Отказано в доступе **550 5.7.520,** ваша организация не разрешает внешнюю перенастройку", убедитесь, что политика настроена, чтобы включить внешний автопропуск.

**Примечание:** Рекомендуется отключить внешнюю автозапружение в политике исходящие фильтры нежелательной почты по умолчанию и включить ее только для пользователей, которым требуется внешняя переадружение, создав настраиваемую политику для этих пользователей. Дополнительные тексты можно прочитать в настройках внешней переадстройки электронной почты [в Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)