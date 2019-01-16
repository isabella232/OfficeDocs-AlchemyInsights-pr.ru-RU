---
title: Изменение NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: b296e76c3d39cad16f329215f0480ae260e77f2e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308573"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="5d2de-102">Обновление серверов доменных имен для Office 365</span><span class="sxs-lookup"><span data-stu-id="5d2de-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="5d2de-103">Примечание: Изменениям имен в некоторых случаях может потребоваться до 48 часов для распространения.</span><span class="sxs-lookup"><span data-stu-id="5d2de-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5d2de-p101">Чтобы настроить домен в Office 365, необходимо обновить серверы доменных имен у регистратора. Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="5d2de-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5d2de-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="5d2de-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="5d2de-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="5d2de-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="5d2de-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5d2de-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="5d2de-109">NS2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5d2de-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="5d2de-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="5d2de-110">Save changes.</span></span>
    
<span data-ttu-id="5d2de-111">Подробные инструкции также можно найти в следующей статье: [Изменение серверов доменных имен для настройки Office 365 у любого регистратора доменных имен](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="5d2de-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

