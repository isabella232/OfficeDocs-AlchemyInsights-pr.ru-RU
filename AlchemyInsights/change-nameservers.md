---
title: Изменение серверов доменных имен
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706768"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="c97e0-102">Обновление серверов доменных имен для указания на системы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c97e0-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="c97e0-103">Примечание. Распространение изменений серверов доменных имен иногда может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="c97e0-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="c97e0-p101">Чтобы настроить домен в Microsoft 365, необходимо обновить серверы доменных имен у регистратора. Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="c97e0-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="c97e0-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="c97e0-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="c97e0-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="c97e0-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="c97e0-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c97e0-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="c97e0-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c97e0-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="c97e0-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="c97e0-110">Save changes.</span></span>

<span data-ttu-id="c97e0-111">Подробные инструкции также можно найти в статье [Изменение серверов доменных имен у любого регистратора доменных имен](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="c97e0-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  