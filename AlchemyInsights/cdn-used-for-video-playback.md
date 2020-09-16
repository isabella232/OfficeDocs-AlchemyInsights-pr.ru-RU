---
title: CDN (сеть доставки содержимого), используемая для воспроизведения видеороликов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 6bc87783375a206a84c96eb7ddd58db5bfd31728
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756980"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="d7b42-102">CDN (сеть доставки содержимого), используемая для воспроизведения видеороликов</span><span class="sxs-lookup"><span data-stu-id="d7b42-102">CDN used for video playback</span></span>

<span data-ttu-id="d7b42-103">Прямые трансляции из Stream и внешнего приложения или прямые трансляции с устройства из Yammer/Teams будут автоматически использовать Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="d7b42-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="d7b42-104">Видеоролики по запросу, загруженные в Stream, пока не используют Azure CDN для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="d7b42-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="d7b42-105">Видеоролики, не являющиеся прямыми трансляциями в Stream, воспроизводятся на исходном сервере Azure Media Services, связанном с вашим клиентом в географическом регионе вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="d7b42-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="d7b42-106">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="d7b42-106">For more information, see:</span></span>

- [<span data-ttu-id="d7b42-107">CDN (сеть доставки содержимого), используемая для воспроизведения видеороликов</span><span class="sxs-lookup"><span data-stu-id="d7b42-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
