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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506456"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23

Проверьте запись DNS SPF для домена на общедоступном средстве проверки подлинности или записи DNS в Интернете.

Убедитесь, что исходящее сообщение не было определено как спам корпорацией Майкрософт и направляется через [пул доставки с высоким уровнем риска](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Сообщения в пуле доставки с высоким уровнем риска не проходят проверку SPF и, следовательно, не принимаются конечной организацией электронной почты.

Если проблема не исчезнет, обратитесь к администратору почтового узла, на который вы пытаетесь отправить сообщение. Запишите подробную внешнюю ошибку, доступную в сообщении Bounce. Служба поддержки Майкрософт, возможно, не сможет помочь.
