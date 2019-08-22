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
ms.openlocfilehash: 3dd96a9731cfd75882dd3bb397005b19d471c882
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531372"
---
# <a name="verify-your-domain"></a><span data-ttu-id="29f36-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="29f36-102">Verify your domain</span></span>

 <span data-ttu-id="29f36-103">**Запись, вероятно, не была обновлена в Интернете.**</span><span class="sxs-lookup"><span data-stu-id="29f36-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="29f36-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="29f36-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="29f36-105">Если вы уже ожидали время, убедитесь, что вы скопировали и вставили точное значение в запись проверки TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="29f36-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="29f36-106">Часто пользователи забывают указать "MS =".</span><span class="sxs-lookup"><span data-stu-id="29f36-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="29f36-107">Эта часть тоже нужна!</span><span class="sxs-lookup"><span data-stu-id="29f36-107">We need that too!</span></span>

- <span data-ttu-id="29f36-108">На некоторых узлах DNS необходимо выполнить дополнительное действие для сохранения файла зоны (в котором хранится запись DNS), чтобы он обновился в Интернете.</span><span class="sxs-lookup"><span data-stu-id="29f36-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="29f36-109">Убедитесь, что вы сохранили изменения, чтобы у Office 365 появилась возможность увидеть и проверить запись.</span><span class="sxs-lookup"><span data-stu-id="29f36-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
