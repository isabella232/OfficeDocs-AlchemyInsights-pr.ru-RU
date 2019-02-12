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
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 7332650d1763e2bbd13be48f406fb04b8849a6c1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29911245"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a7eac-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="a7eac-102">Verify your domain</span></span>

 <span data-ttu-id="a7eac-103">**Запись, вероятно, не обновляется через Интернет.**</span><span class="sxs-lookup"><span data-stu-id="a7eac-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a7eac-104">Обычно новая запись становится доступна через несколько минут, но иногда ее обновление может занять до нескольких часов.</span><span class="sxs-lookup"><span data-stu-id="a7eac-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a7eac-p101">Если ожидал, который уже срок, повторно проверьте, что вы скопировать и вставить точное значение в подтверждающей записи TXT на сервере DNS. Одна проблема распространенных без учета «MS =» в рамках эту запись. Нам нужно, слишком!</span><span class="sxs-lookup"><span data-stu-id="a7eac-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="a7eac-p102">На некоторых серверах DNS необходимо выполнить дополнительные действия для сохраните файл зоны (где хранится DNS-запись) таким образом, будет выполнено обновление через Интернет. Убедитесь в том, что изменения были сохранены, можно увидеть и проверки записи Office 365.</span><span class="sxs-lookup"><span data-stu-id="a7eac-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

