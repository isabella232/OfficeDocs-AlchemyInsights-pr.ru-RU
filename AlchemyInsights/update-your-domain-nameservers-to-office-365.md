---
title: Обновление серверов доменных имен для Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742198"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="431b4-102">Обновление серверов доменных имен для Office 365</span><span class="sxs-lookup"><span data-stu-id="431b4-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="431b4-103">Примечание. Распространение изменений серверов доменных имен иногда может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="431b4-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="431b4-p101">Чтобы настроить домен в Office 365, необходимо обновить серверы доменных имен у регистратора. Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="431b4-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="431b4-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="431b4-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="431b4-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="431b4-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="431b4-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="431b4-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="431b4-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="431b4-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="431b4-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="431b4-110">Save changes.</span></span>

<span data-ttu-id="431b4-111">Подробные инструкции также можно найти в следующей статье: [Изменение серверов доменных имен для настройки Office 365 у любого регистратора доменных имен](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="431b4-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  