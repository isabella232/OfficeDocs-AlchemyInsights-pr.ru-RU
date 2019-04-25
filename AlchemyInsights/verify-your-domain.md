---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d215f3af0cf4b46b12c8cb51a9572adb00f354e4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420065"
---
# <a name="verify-your-domain"></a><span data-ttu-id="3ba53-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="3ba53-102">Verify your domain</span></span>

 <span data-ttu-id="3ba53-103">**Запись, вероятно, не была обновлена в Интернете.**</span><span class="sxs-lookup"><span data-stu-id="3ba53-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="3ba53-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="3ba53-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="3ba53-105">Если вы уже ожидали время, убедитесь, что вы скопировали и вставили точное значение в запись проверки TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="3ba53-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="3ba53-106">Часто пользователи забывают указать "MS =".</span><span class="sxs-lookup"><span data-stu-id="3ba53-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="3ba53-107">Эта часть тоже нужна!</span><span class="sxs-lookup"><span data-stu-id="3ba53-107">We need that too!</span></span>
    
- <span data-ttu-id="3ba53-108">На некоторых узлах DNS необходимо выполнить дополнительное действие для сохранения файла зоны (в котором хранится запись DNS), чтобы он обновился в Интернете.</span><span class="sxs-lookup"><span data-stu-id="3ba53-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="3ba53-109">Убедитесь, что вы сохранили изменения, чтобы у Office 365 появилась возможность увидеть и проверить запись.</span><span class="sxs-lookup"><span data-stu-id="3ba53-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

