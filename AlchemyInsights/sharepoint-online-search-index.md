---
title: Поиск в SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 85f29fabe3189fe248696155208b56d4901ab6de
ms.sourcegitcommit: b5370f0fc8da1e7e5ac960cb622a21612a9c86be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/29/2020
ms.locfileid: "42341114"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="70270-102">Обход контента и индексирование в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="70270-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="70270-103">Контент должен обходиться и добавляться в индекс поиска, чтобы пользователи могли найти то, что ищете в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="70270-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="70270-104">Убедитесь, что контент сайта можно найти, выполнив [Поиск контента сайта](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="70270-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="70270-105">При изменении управляемого свойства или сопоставления свойств для обхода и управляемых свойств необходимо выполнить повторный обход контента сайта для отображения изменений в индексе поиска.</span><span class="sxs-lookup"><span data-stu-id="70270-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="70270-106">Дополнительные сведения см. в статье [запрос на обход и повторная индексация сайта, библиотеки или списка вручную](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="70270-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="70270-107">Подождите как минимум 24 часа после ручного запроса обхода контента и полного повторного индексирования, чтобы проверить, не возникла ли проблема.</span><span class="sxs-lookup"><span data-stu-id="70270-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="70270-108">Если после начала обхода контента и полного повторного индексирования прошло более 24 часов, запишите в журнал обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="70270-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="70270-109">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="70270-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="70270-110">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="70270-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="70270-111">**Важно!** если сайт, документ (библиотека) или список был удален и по-прежнему отображается в результатах поиска, при попытке доступа к нему пользователи должны получить **файл ошибки 404, не найденный** .</span><span class="sxs-lookup"><span data-stu-id="70270-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="70270-112">Эта проблема должна быть зарегистрирована в журнале поддержки для дальнейшего изучения.</span><span class="sxs-lookup"><span data-stu-id="70270-112">This issue should be logged as a support case for further investigation.</span></span>



