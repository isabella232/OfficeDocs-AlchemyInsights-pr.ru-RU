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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676510"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23

Проверьте запись DNS SPF для домена на общедоступном средстве проверки подлинности или записи DNS в Интернете.

Убедитесь, что исходящее сообщение не было определено как спам корпорацией Майкрософт и направляется через [пул доставки с высоким уровнем риска](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Сообщения в пуле доставки с высоким уровнем риска не проходят проверку SPF и, следовательно, не принимаются конечной организацией электронной почты.

Если проблема не исчезнет, обратитесь к администратору почтового узла, на который вы пытаетесь отправить сообщение. Запишите подробную внешнюю ошибку, доступную в сообщении Bounce. Служба поддержки Майкрософт, возможно, не сможет помочь.
