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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="80e2e-102">Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="80e2e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="80e2e-103">Проверьте запись SPF DNS для вашего домена в общедоступных SPF или DNS-регистраторе в Интернете.</span><span class="sxs-lookup"><span data-stu-id="80e2e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="80e2e-104">Убедитесь, что исходящие сообщения не были идентифицированы корпорацией Майкрософт как нежелательной почты и переназначались через пул доставки с высоким [риском.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="80e2e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="80e2e-105">Сообщения в пуле доставки с высоким уровнем риска не будут проходить проверки SPF и поэтому не будут приниматься организацией электронной почты назначения.</span><span class="sxs-lookup"><span data-stu-id="80e2e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="80e2e-106">Если проблема сохраняется, может потребоваться связаться с администратором почтового хозяйского сайта, к которому вы отправляете электронную почту.</span><span class="sxs-lookup"><span data-stu-id="80e2e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="80e2e-107">Обратите внимание на детальную внешнюю ошибку, доступную в сообщении отказов.</span><span class="sxs-lookup"><span data-stu-id="80e2e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="80e2e-108">Поддержка Майкрософт может оказаться не в состоянии помочь в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="80e2e-108">Microsoft support may not be able to assist further.</span></span>
