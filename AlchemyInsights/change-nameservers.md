---
title: Изменение NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 1b49321d3bcc066136080da09be6d534ec3c3bbb
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912839"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="9942d-102">Обновление серверов доменных имен для Office 365</span><span class="sxs-lookup"><span data-stu-id="9942d-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="9942d-103">Примечание: Изменениям имен в некоторых случаях может потребоваться до 48 часов для распространения.</span><span class="sxs-lookup"><span data-stu-id="9942d-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="9942d-p101">Чтобы настроить домен в Office 365, необходимо обновить серверы доменных имен у регистратора. Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="9942d-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="9942d-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="9942d-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="9942d-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="9942d-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="9942d-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="9942d-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="9942d-109">NS2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="9942d-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="9942d-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="9942d-110">Save changes.</span></span>
    
<span data-ttu-id="9942d-111">Подробные инструкции также можно найти в следующей статье: [Изменение серверов доменных имен для настройки Office 365 у любого регистратора доменных имен](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="9942d-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

