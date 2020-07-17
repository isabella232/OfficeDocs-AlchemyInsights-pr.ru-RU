---
title: то же самое, что и filename
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750983"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4f546-102">"Обязательный заголовок Алчеми H1, H2's не работает".</span><span class="sxs-lookup"><span data-stu-id="4f546-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="4f546-103">Рекомендации и рекомендации по разработке Алчеми:</span><span class="sxs-lookup"><span data-stu-id="4f546-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4f546-104">**Не публикуйте алчеми Insights в папках**, так как это приведет к нарушению структуры URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4f546-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="4f546-105">Мы хотим устранить эту ошибку.</span><span class="sxs-lookup"><span data-stu-id="4f546-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="4f546-106">Файлы в папке **алчеминсигхтс** должны содержать имена файлов с символами нижнего регистра с дефисами для пробелов ex.</span><span class="sxs-lookup"><span data-stu-id="4f546-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="4f546-107">***Практическое руководство — удержание***.</span><span class="sxs-lookup"><span data-stu-id="4f546-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="4f546-108">Включите идентификатор правила или идентификатор контейнера из [портала партнеров алчеми](https://alchemyportal.azurewebsites.net) в поле MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="4f546-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="4f546-109">Пример.</span><span class="sxs-lookup"><span data-stu-id="4f546-109">ex.</span></span> <span data-ttu-id="4f546-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="4f546-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="4f546-111">Используйте остальные метаданные вверху этого файла в качестве шаблона.</span><span class="sxs-lookup"><span data-stu-id="4f546-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="4f546-112">На [портале партнера алчеми](https://alchemyportal.azurewebsites.net)перейдите к разделу **Application Insight Title (заголовок клиента** ) и используйте его в качестве отправной точки для получения информации о должности H1.</span><span class="sxs-lookup"><span data-stu-id="4f546-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4f546-113">В верхней части алчеми Insights должен быть только один элемент H1, или они будут прерываться в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="4f546-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="4f546-114">H2S не отображаются, поэтому для обозначения отдельных разделов используйте **полужирное начертание** или другие условные обозначения.</span><span class="sxs-lookup"><span data-stu-id="4f546-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4f546-115">Затем заполните основной текст, используя черновик материала в разделе "сведения о клиентах" страницы правила Алчеми</span><span class="sxs-lookup"><span data-stu-id="4f546-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4f546-116">Маркированные списки прекрасно отличаются</span><span class="sxs-lookup"><span data-stu-id="4f546-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4f546-117">Слишком нумерованные списки</span><span class="sxs-lookup"><span data-stu-id="4f546-117">Numbered lists too</span></span>
    1. <span data-ttu-id="4f546-118">**Полужирный** и *курсив* — это хорошо</span><span class="sxs-lookup"><span data-stu-id="4f546-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4f546-119">Ссылки всегда должны быть ссылками **на веб-/Екстернал** или **глубокими ссылками на элементы пользовательского интерфейса**, а не внутренними ссылками.</span><span class="sxs-lookup"><span data-stu-id="4f546-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="4f546-120">На данный момент фотографии не поддерживаются официально, но они включены в схему.</span><span class="sxs-lookup"><span data-stu-id="4f546-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="4f546-121">И это уже слишком большая длина.</span><span class="sxs-lookup"><span data-stu-id="4f546-121">And this is really already a bit too long.</span></span> <span data-ttu-id="4f546-122">Рекомендация: около 400 символов---------------------------------</span><span class="sxs-lookup"><span data-stu-id="4f546-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4f546-123">Когда контент будет готов, изтяните его в ветвь Live.</span><span class="sxs-lookup"><span data-stu-id="4f546-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="4f546-124">Затем перейдите на [портал партнера алчеми](https://alchemyportal.azurewebsites.net) и введите имя файла в поле URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="4f546-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 