---
title: Защиты от спама — 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717338"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="b394d-102">Устранение проблем с доставкой электронной почты для кода ошибки 5.7.23</span><span class="sxs-lookup"><span data-stu-id="b394d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="b394d-103">Проверьте запись DNS SPF для домена на общедоступном средстве проверки подлинности или записи DNS в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b394d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="b394d-104">Убедитесь, что исходящее сообщение не было определено как спам корпорацией Майкрософт и направляется через [пул доставки с высоким уровнем риска](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="b394d-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="b394d-105">Сообщения в пуле доставки с высоким уровнем риска не проходят проверку SPF и, следовательно, не принимаются конечной организацией электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b394d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="b394d-106">Если проблема не исчезнет, обратитесь к администратору почтового узла, на который вы пытаетесь отправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="b394d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="b394d-107">Запишите подробную внешнюю ошибку, доступную в сообщении Bounce.</span><span class="sxs-lookup"><span data-stu-id="b394d-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="b394d-108">Служба поддержки Майкрософт, возможно, не сможет помочь.</span><span class="sxs-lookup"><span data-stu-id="b394d-108">Microsoft support may not be able to assist further.</span></span>
