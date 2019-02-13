---
title: 'то же, что имя файла лучше всего подходит [ПРАВИЛА # — описание]'
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
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939318"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="179cd-102">Обязательные Алхимия заголовок H1, H2 не работают.</span><span class="sxs-lookup"><span data-stu-id="179cd-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="179cd-103">Практические советы и рекомендации по разработке Алхимия:</span><span class="sxs-lookup"><span data-stu-id="179cd-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="179cd-p101">**Не могут быть вложенными полезные сведения о Алхимия в папках**— это нарушит работу структуры URL-адресов. Мы искали в это исправление.</span><span class="sxs-lookup"><span data-stu-id="179cd-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="179cd-106">Файлы в папке **AlchemyInsights** должны иметь идентификатор правила и имя правила с [портал партнерских Алхимия](https://alchemyportal.azurewebsites.net) в имени файла.</span><span class="sxs-lookup"><span data-stu-id="179cd-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="179cd-p102">например ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="179cd-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="179cd-p103">Используйте метаданные в верхней части этого файла в качестве шаблона. Ничего не требуется.</span><span class="sxs-lookup"><span data-stu-id="179cd-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="179cd-111">[Портал партнерских Алхимия](https://alchemyportal.azurewebsites.net)перейдите до раздела **клиента возможность получения заголовка:** и использования, выберите пункт начала в качестве названия H1 для сведений об.</span><span class="sxs-lookup"><span data-stu-id="179cd-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="179cd-p104">Алхимия полезные сведения о должны иметь только один H1 вверху или они нарушит работу в рабочей среде. H2s не отображать это так использовать **Полужирный** или другие условные обозначения для обозначения отдельные разделы.</span><span class="sxs-lookup"><span data-stu-id="179cd-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="179cd-114">Затем заполните поля в к основному тексту, с помощью черновой материал в разделе клиента полезные сведения о странице Алхимия правила</span><span class="sxs-lookup"><span data-stu-id="179cd-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="179cd-115">Маркированные списки работают нормально</span><span class="sxs-lookup"><span data-stu-id="179cd-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="179cd-116">Слишком нумерованные списки</span><span class="sxs-lookup"><span data-stu-id="179cd-116">Numbered lists too</span></span>
    1. <span data-ttu-id="179cd-117">**Полужирный** и *Курсив* a-ok</span><span class="sxs-lookup"><span data-stu-id="179cd-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="179cd-118">Ссылки всегда должно быть либо **«URL-ссылки» / внешних** или **глубокое ссылки на элементы пользовательского интерфейса**, не внутренние ссылки.</span><span class="sxs-lookup"><span data-stu-id="179cd-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="179cd-p105">И это действительно еще немного слишком много времени. Около 400 символов — лучше</span><span class="sxs-lookup"><span data-stu-id="179cd-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="179cd-p106">Когда контент готов, его по запросу для ветвления live. Затем перейдите на [портал партнерских Алхимия](https://alchemyportal.azurewebsites.net) и введите имя файла в поле URL-адрес. Убедитесь, что возможность получения проверяются и публикуются отвечает «Да» и выберите правило обновления. **(Это будет выглядеть красивее в новой версии портала - отпускает в ближайшее время.)** 
 ![поля URL-адреса](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="179cd-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

