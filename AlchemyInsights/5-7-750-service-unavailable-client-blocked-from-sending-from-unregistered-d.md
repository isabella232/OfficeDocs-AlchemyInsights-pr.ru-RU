---
title: 1048 служба 5.7.750 недоступна. Клиент блокировал отправку с незарегистрированных доменов
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664255"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="86806-103">5.7.750 Отправка клиентом из незарегистрированного домена заблокирована</span><span class="sxs-lookup"><span data-stu-id="86806-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="86806-104">Ошибка возникает, когда большой объем сообщений отправляется из доменов, которые не были подготовлены в клиенте (добавлены как обслуживаемые домены и проверены).</span><span class="sxs-lookup"><span data-stu-id="86806-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="86806-105">Чтобы избежать этой ошибки, вы можете использовать соединитель почтовых ящиков на основе сертификатов, в котором домен сертификата является подготовленным доменом, или можно подготовить все отправные домены.</span><span class="sxs-lookup"><span data-stu-id="86806-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
