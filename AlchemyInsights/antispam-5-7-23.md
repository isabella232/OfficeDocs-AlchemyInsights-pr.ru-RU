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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821424"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23

Проверьте запись SPF DNS для вашего домена в общедоступных SPF или DNS-регистраторе в Интернете.

Убедитесь, что исходящие сообщения не были идентифицированы корпорацией Майкрософт как нежелательной почты и переназначались через пул доставки с высоким [риском.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Сообщения в пуле доставки с высоким уровнем риска не будут проходить проверки SPF и поэтому не будут приниматься организацией электронной почты назначения.

Если проблема сохраняется, может потребоваться связаться с администратором почтового хозяйского сайта, к которому вы отправляете электронную почту. Обратите внимание на детальную внешнюю ошибку, доступную в сообщении отказов. Поддержка Майкрософт может оказаться не в состоянии помочь в дальнейшем.
