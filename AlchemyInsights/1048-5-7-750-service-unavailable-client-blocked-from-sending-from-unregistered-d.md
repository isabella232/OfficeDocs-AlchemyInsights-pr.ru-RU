---
title: 1048 5.7.750 служба недоступна. Клиент запретом Отправка из незарегистрированных доменов
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.openlocfilehash: 90bcf51f4dd2a8e06065a349a39cb1188b4717ce
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486158"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="ef878-103">5.7.750 клиента запретом незарегистрированных домена</span><span class="sxs-lookup"><span data-stu-id="ef878-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="ef878-104">Эта ошибка возникает при большой объем сообщения отправляются из доменов, которые не подготовлены в Office 365 (добавлен в качестве обслуживаемых доменов и его проверки).</span><span class="sxs-lookup"><span data-stu-id="ef878-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="ef878-105">Чтобы избежать этой ошибки, можно использовать соединитель поток почты на основе сертификатов где сертификат домена подготовленных домена, или вы можете подготовить все домены отправителя.</span><span class="sxs-lookup"><span data-stu-id="ef878-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

