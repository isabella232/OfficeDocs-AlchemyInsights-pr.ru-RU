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
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365430"
---
# <a name="verify-your-domain"></a><span data-ttu-id="27e7e-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="27e7e-102">Verify your domain</span></span>

 <span data-ttu-id="27e7e-103">**Запись, вероятно, не была обновлена в Интернете.**</span><span class="sxs-lookup"><span data-stu-id="27e7e-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="27e7e-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="27e7e-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="27e7e-105">Если вы уже ожидали время, убедитесь, что вы скопировали и вставили точное значение в запись проверки TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="27e7e-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="27e7e-106">Часто пользователи забывают указать "MS =".</span><span class="sxs-lookup"><span data-stu-id="27e7e-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="27e7e-107">Эта часть тоже нужна!</span><span class="sxs-lookup"><span data-stu-id="27e7e-107">We need that too!</span></span>

- <span data-ttu-id="27e7e-108">На некоторых узлах DNS необходимо выполнить дополнительное действие для сохранения файла зоны (в котором хранится запись DNS), чтобы он обновился в Интернете.</span><span class="sxs-lookup"><span data-stu-id="27e7e-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="27e7e-109">Убедитесь, что вы сохранили изменения, чтобы у Office 365 появилась возможность увидеть и проверить запись.</span><span class="sxs-lookup"><span data-stu-id="27e7e-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
