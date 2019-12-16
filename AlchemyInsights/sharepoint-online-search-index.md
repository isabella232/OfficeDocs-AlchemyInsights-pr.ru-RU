---
title: Поиск в SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044056"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="fae87-102">Обход контента и индексирование в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fae87-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="fae87-103">Контент должен обходиться и добавляться в индекс поиска, чтобы пользователи могли найти то, что ищете в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fae87-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="fae87-104">Обход контента выполняется автоматически на основе предварительно определенного расписания обхода (изменение расписания обхода невозможно).</span><span class="sxs-lookup"><span data-stu-id="fae87-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="fae87-105">Программа-обходчик выбирает контент, который изменился с момента последнего обхода, и обновляет индекс.</span><span class="sxs-lookup"><span data-stu-id="fae87-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="fae87-106">Чтобы обеспечить обход контента и обновление индекса, обратите внимание на следующее:</span><span class="sxs-lookup"><span data-stu-id="fae87-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="fae87-107">Убедитесь, что контент сайта можно найти, выполнив [Поиск контента сайта](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="fae87-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="fae87-108">При изменении управляемого свойства или сопоставления свойств для обхода и управляемых свойств необходимо выполнить повторный обход контента сайта для отображения изменений в индексе поиска.</span><span class="sxs-lookup"><span data-stu-id="fae87-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="fae87-109">Так как изменена схема поиска, а не сайт, программа-обходчик не выполнит переиндексацию автоматически.</span><span class="sxs-lookup"><span data-stu-id="fae87-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="fae87-110">Дополнительные сведения см. в статье [запрос на обход и повторная индексация сайта, библиотеки или списка вручную](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="fae87-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="fae87-111">Подождите как минимум 24 часа после ручного запроса обхода контента и полного повторного индексирования, чтобы проверить, не возникла ли проблема.</span><span class="sxs-lookup"><span data-stu-id="fae87-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="fae87-112">Если после начала обхода контента и полного повторного индексирования прошло более 24 часов, запишите в журнал обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="fae87-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="fae87-113">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="fae87-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="fae87-114">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="fae87-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fae87-115">Если сайт, документ (библиотека) или список были удалены и по-прежнему отображаются в результатах поиска, при попытке доступа к нему пользователи должны получить **файл ошибки 404, не найденный** .</span><span class="sxs-lookup"><span data-stu-id="fae87-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="fae87-116">Эта проблема должна быть зарегистрирована в журнале поддержки для дальнейшего изучения.</span><span class="sxs-lookup"><span data-stu-id="fae87-116">This issue should be logged as a support case for further investigation.</span></span> 



