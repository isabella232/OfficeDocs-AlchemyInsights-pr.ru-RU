---
title: Обновление серверов доменных имен для указания на системы Майкрософт
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734924"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="d93c9-102">Обновление серверов доменных имен для указания на системы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="d93c9-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="d93c9-103">Примечание. Распространение изменений серверов доменных имен иногда может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="d93c9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="d93c9-104">Чтобы настроить ваш домен с помощью Microsoft, необходимо обновить серверов доменных имен в регистраторе.</span><span class="sxs-lookup"><span data-stu-id="d93c9-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="d93c9-105">Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="d93c9-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="d93c9-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="d93c9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="d93c9-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="d93c9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="d93c9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d93c9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="d93c9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d93c9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="d93c9-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="d93c9-110">Save changes.</span></span>

<span data-ttu-id="d93c9-111">Подробные инструкции, приведенные в этой статье, можно найти здесь: [изменение серверов доменных имен для настройки Microsoft 365 с помощью любого регистратора доменных](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) имен</span><span class="sxs-lookup"><span data-stu-id="d93c9-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  