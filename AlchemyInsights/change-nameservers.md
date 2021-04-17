---
title: Изменение серверов доменных имен
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818625"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="a9880-102">Обновление серверов доменных имен для указания на системы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="a9880-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="a9880-103">Примечание. Распространение изменений серверов доменных имен иногда может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="a9880-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="a9880-p101">Чтобы настроить домен в Microsoft 365, необходимо обновить серверы доменных имен у регистратора. Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="a9880-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="a9880-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="a9880-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="a9880-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="a9880-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="a9880-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a9880-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="a9880-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a9880-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="a9880-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="a9880-110">Save changes.</span></span>

<span data-ttu-id="a9880-111">Подробные инструкции также можно найти в статье [Изменение серверов доменных имен у любого регистратора доменных имен](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="a9880-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  