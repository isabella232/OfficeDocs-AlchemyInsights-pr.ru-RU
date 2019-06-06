---
title: Управление словарями поиска в SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736065"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="28e22-102">Поиск в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="28e22-102">Search in SharePoint Online</span></span>

<span data-ttu-id="28e22-103">Контент должен обходиться и добавляться в индекс поиска, чтобы пользователи могли найти то, что ищете в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="28e22-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="28e22-104">Обход контента выполняется автоматически на основе предварительно определенного расписания обхода (изменение расписания обхода невозможно).</span><span class="sxs-lookup"><span data-stu-id="28e22-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="28e22-105">Программа-обходчик выбирает контент, который изменился с момента последнего обхода, и обновляет индекс.</span><span class="sxs-lookup"><span data-stu-id="28e22-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="28e22-106">Чтобы обеспечить обход контента и обновление индекса, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="28e22-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="28e22-107">Убедитесь, что контент сайта можно найти, выполнив поиск контента сайта.</span><span class="sxs-lookup"><span data-stu-id="28e22-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="28e22-108">Дополнительную информацию можно узнать в статье [Включение поддержки поиска контента на сайте](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="28e22-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="28e22-109">При изменении управляемого свойства или сопоставления свойств для обхода и управляемых свойств необходимо выполнить повторный обход контента сайта для отображения изменений в индексе поиска.</span><span class="sxs-lookup"><span data-stu-id="28e22-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="28e22-110">Так как изменена схема поиска, а не сайт, программа-обходчик не выполнит переиндексацию автоматически.</span><span class="sxs-lookup"><span data-stu-id="28e22-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="28e22-111">Дополнительные сведения см. в статье [запрос на обход и повторная индексация сайта, библиотеки или списка вручную](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="28e22-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="28e22-112">Подождите как минимум 24 часа после ручного запроса обхода контента и полного повторного индексирования, чтобы проверить, не возникла ли проблема.</span><span class="sxs-lookup"><span data-stu-id="28e22-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="28e22-113">Если после начала обхода контента и полного повторного индексирования прошло более 24 часов, запишите в журнал обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="28e22-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="28e22-114">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="28e22-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="28e22-115">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="28e22-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="28e22-116">**Важно!** если сайт, документ (библиотека) или список был удален и по-прежнему отображается в результатах поиска, при попытке доступа пользователи должны получить файл ошибки 404, который не найден.</span><span class="sxs-lookup"><span data-stu-id="28e22-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="28e22-117">Эта проблема должна быть зарегистрирована в журнале поддержки для дальнейшего изучения.</span><span class="sxs-lookup"><span data-stu-id="28e22-117">This issue should be logged as a support case for further investigation.</span></span> 



