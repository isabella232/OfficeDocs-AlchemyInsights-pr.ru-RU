---
title: Управление схемой поиска в SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270140"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="32fea-102">Управление схемой поиска в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="32fea-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="32fea-103">Схема поиска определяет, какие пользователи могут выполнять поиск, как пользователи могут выполнять поиск, а также как отображать результаты на веб-сайтах поиска.</span><span class="sxs-lookup"><span data-stu-id="32fea-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="32fea-104">В разделе [Управление схемой поиска в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) можно узнать, как:</span><span class="sxs-lookup"><span data-stu-id="32fea-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="32fea-105">Изменение схемы поиска.</span><span class="sxs-lookup"><span data-stu-id="32fea-105">Change the search schema.</span></span>
- <span data-ttu-id="32fea-106">Создание управляемых свойств.</span><span class="sxs-lookup"><span data-stu-id="32fea-106">Create managed properties.</span></span>
- <span data-ttu-id="32fea-107">Сопоставление свойств для обхода карты с обходом контента с управляемыми свойствами.</span><span class="sxs-lookup"><span data-stu-id="32fea-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="32fea-108">Обратите внимание на следующие сведения об управлении схемой поиска.</span><span class="sxs-lookup"><span data-stu-id="32fea-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="32fea-109">Если вы получаете предупреждение о том **, что приложение приостановлено** при изменении схемы, оно будет доступно только в том случае, если происходит обслуживание службы.</span><span class="sxs-lookup"><span data-stu-id="32fea-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="32fea-110">Если прошло более 24 часов и вы по-прежнему используете предупреждение, запишите в журнал обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="32fea-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="32fea-111">При изменении управляемых свойств или добавлении новых изменения вступают в силу только после повторного обхода контента.</span><span class="sxs-lookup"><span data-stu-id="32fea-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="32fea-112">В SharePoint Online обход контента происходит автоматически на основе заданного расписания обхода.</span><span class="sxs-lookup"><span data-stu-id="32fea-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="32fea-113">Чтобы убедиться в том, что вы выполняете обход изменений, вы можете [запрашивать повторную индексацию списка или библиотеки](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="32fea-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="32fea-114">Полный обзор схемы поиска приведен в статье [введение схемы поиска](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="32fea-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


