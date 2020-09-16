---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734319"
---
# <a name="verify-your-domain"></a><span data-ttu-id="06c85-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="06c85-102">Verify your domain</span></span>

 <span data-ttu-id="06c85-103">**Запись, вероятно, не была обновлена в Интернете.**</span><span class="sxs-lookup"><span data-stu-id="06c85-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="06c85-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="06c85-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="06c85-105">Если вы уже ожидали время, убедитесь, что вы скопировали и вставили точное значение в запись проверки TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="06c85-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="06c85-106">Часто пользователи забывают указать "MS =".</span><span class="sxs-lookup"><span data-stu-id="06c85-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="06c85-107">Эта часть тоже нужна!</span><span class="sxs-lookup"><span data-stu-id="06c85-107">We need that too!</span></span>

- <span data-ttu-id="06c85-108">На некоторых узлах DNS необходимо выполнить дополнительное действие для сохранения файла зоны (в котором хранится запись DNS), чтобы он обновился в Интернете.</span><span class="sxs-lookup"><span data-stu-id="06c85-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="06c85-109">Убедитесь, что вы сохранили изменения, чтобы Майкрософт могли просматривать и проверять запись.</span><span class="sxs-lookup"><span data-stu-id="06c85-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
