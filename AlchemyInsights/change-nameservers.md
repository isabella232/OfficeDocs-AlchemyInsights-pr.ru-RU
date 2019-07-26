---
title: Изменение серверов доменных имен
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902942"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="09571-102">Обновление серверов доменных имен для Office 365</span><span class="sxs-lookup"><span data-stu-id="09571-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="09571-103">Примечание. Распространение изменений серверов доменных имен иногда может занять до 48 часов.</span><span class="sxs-lookup"><span data-stu-id="09571-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="09571-p101">Чтобы настроить домен в Office 365, необходимо обновить серверы доменных имен у регистратора. Создайте или измените записи серверов доменных имен у своего регистратора.</span><span class="sxs-lookup"><span data-stu-id="09571-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="09571-106">Найдите на веб-сайте регистратора домена раздел, где можно изменять серверы доменных имен.</span><span class="sxs-lookup"><span data-stu-id="09571-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="09571-107">Настройте две записи серверов доменных имен с приведенными ниже значениями.</span><span class="sxs-lookup"><span data-stu-id="09571-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="09571-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="09571-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="09571-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="09571-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="09571-110">Сохраните изменения.</span><span class="sxs-lookup"><span data-stu-id="09571-110">Save changes.</span></span>

<span data-ttu-id="09571-111">Подробные инструкции также можно найти в следующей статье: [Изменение серверов доменных имен для настройки Office 365 у любого регистратора доменных имен](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="09571-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  