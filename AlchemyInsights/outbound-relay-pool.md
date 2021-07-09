---
title: Исходящие пулы ретрансляции
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339982"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="1aced-102">Исходящие пулы ретрансляции</span><span class="sxs-lookup"><span data-stu-id="1aced-102">Outbound relay pool</span></span>

<span data-ttu-id="1aced-103">Корпорация Майкрософт внося некоторые изменения в конфигурацию для ретрансляции или отправки электронной почты через Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1aced-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="1aced-104">Сообщения в определенных сценариях передаются или передаются через Microsoft 365 с помощью специального пула ретрансляторов.</span><span class="sxs-lookup"><span data-stu-id="1aced-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="1aced-105">Сообщения, отправленные с помощью пула ретрансляторов, могут конечном итоге ложиться в папку нежелательной почты получателя.</span><span class="sxs-lookup"><span data-stu-id="1aced-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="1aced-106">Дополнительные сведения см. в [пулах исходящие доставки](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="1aced-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="1aced-107">Чтобы избежать сценария с помощью пула ретрансляторов, убедитесь, что переадтрансляции и ретрансляции сообщений соответствуют одному из следующих критериев:</span><span class="sxs-lookup"><span data-stu-id="1aced-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="1aced-108">Исходящие отправитель — это принятый домен клиента.</span><span class="sxs-lookup"><span data-stu-id="1aced-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="1aced-109">Система политики отправитель (SPF) передается, когда сообщение поступает Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1aced-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="1aced-110">DomainKeys Identified Mail (DKIM) на домене отправитель P2 передается, когда сообщение приходит к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1aced-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="1aced-111">Сообщения, которые соответствуют вышеуказанным критериям, не передаются через пул ретрансляторов.</span><span class="sxs-lookup"><span data-stu-id="1aced-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="1aced-112">Если запись MX для вашего домена указывается на сторонний или локальной сервер, используйте усиленную фильтрацию, чтобы убедиться, что проверка SPF является правильной для входящие сообщения электронной почты и чтобы избежать отправки электронной почты через пул ретрансляторов.</span><span class="sxs-lookup"><span data-stu-id="1aced-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="1aced-113">**Как узнать, влияет ли на нас пул ретрансляторов?**</span><span class="sxs-lookup"><span data-stu-id="1aced-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="1aced-114">Если отправленные или переданные сообщения электронной почты используют один из вышеуказанных критериев, сообщения не будут переданы через пул ретрансляторов.</span><span class="sxs-lookup"><span data-stu-id="1aced-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="1aced-115">Однако если сообщение отправляется через пул ретрансляторов, IP-адрес исходящие серверы находится в диапазоне 40.95.0.0/16, а имя исходящие сервера включает **rly** в имя.</span><span class="sxs-lookup"><span data-stu-id="1aced-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

