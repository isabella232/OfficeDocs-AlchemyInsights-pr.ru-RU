---
title: Поиск в SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770780"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="c41f9-102">Обход контента и индексирование в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c41f9-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="c41f9-103">Контент должен обходиться и добавляться в индекс поиска, чтобы пользователи могли найти то, что ищете в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c41f9-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="c41f9-104">Убедитесь, что контент сайта можно найти, выполнив [Поиск контента сайта](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="c41f9-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="c41f9-105">При изменении управляемого свойства или сопоставления свойств для обхода и управляемых свойств необходимо выполнить повторный обход контента сайта для отображения изменений в индексе поиска.</span><span class="sxs-lookup"><span data-stu-id="c41f9-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="c41f9-106">Дополнительные сведения см. в статье [запрос на обход и повторная индексация сайта, библиотеки или списка вручную](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="c41f9-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="c41f9-107">Подождите как минимум 24 часа после ручного запроса обхода контента и полного повторного индексирования, чтобы проверить, не возникла ли проблема.</span><span class="sxs-lookup"><span data-stu-id="c41f9-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="c41f9-108">Если после начала обхода контента и полного повторного индексирования прошло более 24 часов, запишите в журнал обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="c41f9-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="c41f9-109">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="c41f9-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c41f9-110">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="c41f9-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="c41f9-111">**Важно!** если сайт, документ (библиотека) или список был удален и по-прежнему отображается в результатах поиска, при попытке доступа к нему пользователи должны получить **файл ошибки 404, не найденный** .</span><span class="sxs-lookup"><span data-stu-id="c41f9-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="c41f9-112">Эта проблема должна быть зарегистрирована в журнале поддержки для дальнейшего изучения.</span><span class="sxs-lookup"><span data-stu-id="c41f9-112">This issue should be logged as a support case for further investigation.</span></span>



