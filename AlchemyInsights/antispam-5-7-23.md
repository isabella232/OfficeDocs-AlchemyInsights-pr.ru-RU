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
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="c1b76-102">Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="c1b76-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="c1b76-103">Проверьте запись DNS SPF для домена на общедоступном средстве проверки подлинности или записи DNS в Интернете.</span><span class="sxs-lookup"><span data-stu-id="c1b76-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="c1b76-104">Убедитесь, что исходящее сообщение не было определено как спам в Office 365 и направляется через [пул доставки с высоким уровнем риска](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="c1b76-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="c1b76-105">Сообщения в пуле доставки с высоким уровнем риска не проходят проверку SPF и, следовательно, не принимаются конечной организацией электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c1b76-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="c1b76-106">Если проблема не исчезнет, обратитесь к администратору почтового узла, на который вы пытаетесь отправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="c1b76-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="c1b76-107">Запишите подробную внешнюю ошибку, доступную в сообщении Bounce.</span><span class="sxs-lookup"><span data-stu-id="c1b76-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="c1b76-108">Поддержка Office 365 может быть недоступна для дальнейшей помощи.</span><span class="sxs-lookup"><span data-stu-id="c1b76-108">Office 365 support may not be able to assist further.</span></span>