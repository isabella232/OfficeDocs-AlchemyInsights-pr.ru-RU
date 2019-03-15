---
title: 'то же самое, что и имя_файла лучше [RULE #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634517"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="7d79f-102">Обязательный заголовок Алчеми H1, H2's не работают.</span><span class="sxs-lookup"><span data-stu-id="7d79f-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="7d79f-103">Рекомендации и рекомендации по разработке Алчеми:</span><span class="sxs-lookup"><span data-stu-id="7d79f-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="7d79f-104">**Не публикуйте алчеми Insights в папках**, так как это приведет к нарушению структуры URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="7d79f-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="7d79f-105">Мы хотим устранить эту ошибку.</span><span class="sxs-lookup"><span data-stu-id="7d79f-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="7d79f-106">Файлы в папке **алчеминсигхтс** должны иметь идентификатор правила и имя правила из [алчеми партнерского портала](https://alchemyportal.azurewebsites.net) в имени файла.</span><span class="sxs-lookup"><span data-stu-id="7d79f-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="7d79f-107">Пример.</span><span class="sxs-lookup"><span data-stu-id="7d79f-107">ex.</span></span> <span data-ttu-id="7d79f-108">***976 — инструкции по включению, судебное удержание***</span><span class="sxs-lookup"><span data-stu-id="7d79f-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="7d79f-109">Используйте метаданные, расположенные в верхней части этого файла, в качестве шаблона.</span><span class="sxs-lookup"><span data-stu-id="7d79f-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="7d79f-110">Другие действия не требуются.</span><span class="sxs-lookup"><span data-stu-id="7d79f-110">Nothing else is required.</span></span>
1. <span data-ttu-id="7d79f-111">На [портале партнера алчеми](https://alchemyportal.azurewebsites.net)перейдите к разделу **Application Insight Title (заголовок клиента** ) и используйте его в качестве отправной точки для получения информации о должности H1.</span><span class="sxs-lookup"><span data-stu-id="7d79f-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="7d79f-112">В верхней части Алчеми Insights должен быть только один элемент H1, или они будут прерываться в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="7d79f-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="7d79f-113">H2S не отображаются, поэтому для \*\*\*\* обозначения отдельных разделов используйте полужирное начертание или другие условные обозначения.</span><span class="sxs-lookup"><span data-stu-id="7d79f-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="7d79f-114">Затем заполните основной текст, используя черновик материала в разделе "сведения о клиентах" страницы правила Алчеми</span><span class="sxs-lookup"><span data-stu-id="7d79f-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="7d79f-115">Маркированные списки прекрасно отличаются</span><span class="sxs-lookup"><span data-stu-id="7d79f-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="7d79f-116">Слишком нумерованные списки</span><span class="sxs-lookup"><span data-stu-id="7d79f-116">Numbered lists too</span></span>
    1. <span data-ttu-id="7d79f-117">**Полужирный** и *курсив* — это хорошо</span><span class="sxs-lookup"><span data-stu-id="7d79f-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="7d79f-118">Ссылки всегда должны быть ссылками **на веб-/Екстернал** или **глубокими ссылками на элементы пользовательского интерфейса**, а не внутренними ссылками.</span><span class="sxs-lookup"><span data-stu-id="7d79f-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="7d79f-119">И это уже слишком большая длина.</span><span class="sxs-lookup"><span data-stu-id="7d79f-119">And this is really already a bit too long.</span></span> <span data-ttu-id="7d79f-120">Рекомендация: около 400 символов---------------------------------</span><span class="sxs-lookup"><span data-stu-id="7d79f-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="7d79f-121">Когда контент будет готов, изтяните его в ветвь Live.</span><span class="sxs-lookup"><span data-stu-id="7d79f-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="7d79f-122">Затем перейдите на [портал партнера алчеми](https://alchemyportal.azurewebsites.net) и введите имя файла в поле URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="7d79f-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="7d79f-123">Убедитесь, что проверка и публикация опубликованы: "Да", а затем щелкните Обновить правило.</span><span class="sxs-lookup"><span data-stu-id="7d79f-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="7d79f-124">**(В скором времени в новой версии портала будет отображаться преттиер.)** 
 ![](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="7d79f-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

