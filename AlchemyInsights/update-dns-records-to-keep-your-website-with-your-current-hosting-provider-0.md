---
title: Обновление DNS-записей для сохранения веб-сайта у текущего поставщика услуг размещения веб-сайтов
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827544"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="60c95-102">Обновление DNS-записей для сохранения веб-сайта у текущего поставщика услуг размещения веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="60c95-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="60c95-103">В центре администрирования Microsoft 365 перейдите на страницу **Setup** Domains, а в списке доменов выберите домен, который используется  >  [](https://admin.microsoft.com/Adminportal#/Domains) для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="60c95-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="60c95-104">Нажмите кнопку **+ Создать настраиваемую запись** и введите указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="60c95-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="60c95-105">В поле **Тип DNS** введите **A (адрес)**.</span><span class="sxs-lookup"><span data-stu-id="60c95-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="60c95-106">В поле **Имя узла или псевдоним** введите **@**.</span><span class="sxs-lookup"><span data-stu-id="60c95-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="60c95-107">В поле **IP-адрес** введите текущий IP-адрес веб-сайта, например 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="60c95-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="60c95-p101">Это должен быть  *статический*  , а не  *динамический*  IP-адрес веб-сайта. Уточнить возможность получения статического IP-адреса можно у поставщика услуг размещения, у которого находится ваш общедоступный веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="60c95-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="60c95-110">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="60c95-110">Select **Save**.</span></span>

<span data-ttu-id="60c95-111">Кроме того, можно создать запись CNAME, чтобы упростить поиск веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="60c95-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="60c95-112">Нажмите кнопку **+ Создать настраиваемую запись** и введите указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="60c95-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="60c95-113">В поле **Тип DNS** введите **CNAME (псевдоним)**.</span><span class="sxs-lookup"><span data-stu-id="60c95-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="60c95-114">В поле **Имя узла или псевдоним** введите **www**.</span><span class="sxs-lookup"><span data-stu-id="60c95-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="60c95-115">В качестве значения **Адрес "указывает на"** введите полное доменное имя (FQDN) своего веб-сайта, например contoso.com.</span><span class="sxs-lookup"><span data-stu-id="60c95-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="60c95-116">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="60c95-116">Select **Save**.</span></span>
