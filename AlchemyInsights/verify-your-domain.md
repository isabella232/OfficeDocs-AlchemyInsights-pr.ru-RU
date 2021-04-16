---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771004"
---
# <a name="verify-your-domain"></a><span data-ttu-id="6112d-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="6112d-102">Verify your domain</span></span>

 <span data-ttu-id="6112d-103">**Запись, вероятно, не обновилась в Интернете.**</span><span class="sxs-lookup"><span data-stu-id="6112d-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="6112d-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="6112d-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="6112d-105">Если вы уже так долго ждали, перепроверяйте, что вы скопировали и вклеили точное значение в запись проверки TXT на вашем DNS-хозяйте.</span><span class="sxs-lookup"><span data-stu-id="6112d-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="6112d-106">Часто пользователи забывают указать "MS =".</span><span class="sxs-lookup"><span data-stu-id="6112d-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="6112d-107">Эта часть тоже нужна!</span><span class="sxs-lookup"><span data-stu-id="6112d-107">We need that too!</span></span>

- <span data-ttu-id="6112d-108">На некоторых узлах DNS необходимо выполнить дополнительное действие для сохранения файла зоны (в котором хранится запись DNS), чтобы он обновился в Интернете.</span><span class="sxs-lookup"><span data-stu-id="6112d-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="6112d-109">Убедитесь, что вы сохранили свои изменения, чтобы Корпорация Майкрософт видела и проверяла запись.</span><span class="sxs-lookup"><span data-stu-id="6112d-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
