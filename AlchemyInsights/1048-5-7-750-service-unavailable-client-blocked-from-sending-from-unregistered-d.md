---
title: 1048 5.7.750 служба недоступна. Клиент запретом Отправка из незарегистрированных доменов
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.openlocfilehash: 5fe5b343d89c49e1805e4d0cac6698ef35e1dd30
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921937"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="7326c-103">5.7.750 клиента запретом незарегистрированных домена</span><span class="sxs-lookup"><span data-stu-id="7326c-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="7326c-104">Эта ошибка возникает при большой объем сообщения отправляются из доменов, которые не подготовлены в Office 365 (добавлен в качестве обслуживаемых доменов и его проверки).</span><span class="sxs-lookup"><span data-stu-id="7326c-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="7326c-105">Чтобы избежать этой ошибки, можно использовать соединитель поток почты на основе сертификатов где сертификат домена подготовленных домена, или вы можете подготовить все домены отправителя.</span><span class="sxs-lookup"><span data-stu-id="7326c-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

