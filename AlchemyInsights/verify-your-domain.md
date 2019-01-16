---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307858"
---
# <a name="verify-your-domain"></a><span data-ttu-id="e6695-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="e6695-102">Verify your domain</span></span>

 <span data-ttu-id="e6695-103">**Запись, вероятно, не обновляется через Интернет.**</span><span class="sxs-lookup"><span data-stu-id="e6695-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="e6695-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="e6695-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="e6695-p101">Если ожидал, который уже срок, повторно проверьте, что вы скопировать и вставить точное значение в подтверждающей записи TXT на сервере DNS. Одна проблема распространенных без учета «MS =» в рамках эту запись. Нам нужно, слишком!</span><span class="sxs-lookup"><span data-stu-id="e6695-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="e6695-p102">На некоторых серверах DNS необходимо выполнить дополнительные действия для сохраните файл зоны (где хранится DNS-запись) таким образом, будет выполнено обновление через Интернет. Убедитесь в том, что изменения были сохранены, можно увидеть и проверки записи Office 365.</span><span class="sxs-lookup"><span data-stu-id="e6695-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

