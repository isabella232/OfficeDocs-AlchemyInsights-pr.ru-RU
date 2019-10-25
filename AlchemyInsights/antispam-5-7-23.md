---
title: Защиты от спама — 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682266"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23

Проверьте запись DNS SPF для домена на общедоступном средстве проверки подлинности или записи DNS в Интернете.

Убедитесь, что исходящее сообщение не было определено как спам в Office 365 и направляется через [пул доставки с высоким уровнем риска](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Сообщения в пуле доставки с высоким уровнем риска не проходят проверку SPF и, следовательно, не принимаются конечной организацией электронной почты.

Если проблема не исчезнет, обратитесь к администратору почтового узла, на который вы пытаетесь отправить сообщение. Запишите подробную внешнюю ошибку, доступную в сообщении Bounce.  Поддержка Office 365 может быть недоступна для дальнейшей помощи.