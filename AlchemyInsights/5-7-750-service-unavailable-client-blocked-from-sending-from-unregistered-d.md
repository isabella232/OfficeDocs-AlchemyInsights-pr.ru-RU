---
title: 1048 служба 5.7.750 недоступна. Клиент блокировал отправку с незарегистрированных доменов
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 9417fef2584e9b81a2ca71cbcc5e23ce093d94e8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751716"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="286c4-103">Клиент 5.7.750 блокировал отправку от незарегистрированного домена</span><span class="sxs-lookup"><span data-stu-id="286c4-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="286c4-104">Ошибка возникает, когда большой объем сообщений отправляется из доменов, не подготовленных в Office 365 (добавленные как обслуживаемые домены и проверены).</span><span class="sxs-lookup"><span data-stu-id="286c4-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="286c4-105">Чтобы избежать этой ошибки, вы можете использовать соединитель почтовых ящиков на основе сертификатов, в котором домен сертификата является подготовленным доменом, или можно подготовить все отправные домены.</span><span class="sxs-lookup"><span data-stu-id="286c4-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
