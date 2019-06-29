---
title: Обновление DNS-записей для сохранения веб-сайта у текущего поставщика услуг размещения веб-сайтов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353190"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="c3f5a-102">Обновление DNS-записей для сохранения веб-сайта у текущего поставщика услуг размещения веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="c3f5a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="c3f5a-103">На странице [Домены](https://portal.office.com/adminportal/home#/Domains) в списке доменов выберите домен, который используете для своего веб-сайта, а затем щелкните **Параметры DNS** на панели управления.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="c3f5a-104">Нажмите кнопку **+ Создать настраиваемую запись** и введите указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c3f5a-105">В поле **Тип DNS** введите **A (адрес)**.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="c3f5a-106">В поле **Имя узла или псевдоним** введите **@**.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="c3f5a-107">В поле **IP-адрес** введите текущий IP-адрес веб-сайта, например 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="c3f5a-p101">Это должен быть  *статический*  , а не  *динамический*  IP-адрес веб-сайта. Уточнить возможность получения статического IP-адреса можно у поставщика услуг размещения, у которого находится ваш общедоступный веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="c3f5a-110">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-110">Select **Save**.</span></span>

<span data-ttu-id="c3f5a-111">Кроме того, можно создать запись CNAME, чтобы упростить поиск веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="c3f5a-112">Нажмите кнопку **+ Создать настраиваемую запись** и введите указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="c3f5a-113">В поле **Тип DNS** введите **CNAME (псевдоним)**.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="c3f5a-114">В поле **Имя узла или псевдоним** введите **www**.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="c3f5a-115">В качестве значения **Адрес "указывает на"** введите полное доменное имя (FQDN) своего веб-сайта, например contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="c3f5a-116">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c3f5a-116">Select **Save**.</span></span>
