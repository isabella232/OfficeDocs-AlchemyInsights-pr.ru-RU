---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932182"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23

Проверьте запись SPF DNS для вашего домена в общедоступных SPF или DNS-регистраторе в Интернете.

Убедитесь, что исходящие сообщения не были идентифицированы корпорацией Майкрософт как нежелательной почты и переназначались через пул доставки с высоким [риском.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Сообщения в пуле доставки с высоким уровнем риска не будут проходить проверки SPF и поэтому не будут приниматься организацией электронной почты назначения.

Если проблема сохраняется, может потребоваться связаться с администратором почтового хозяйского сайта, к которому вы отправляете электронную почту. Обратите внимание на детальную внешнюю ошибку, доступную в сообщении отказов. Поддержка Майкрософт может оказаться не в состоянии помочь в дальнейшем.
