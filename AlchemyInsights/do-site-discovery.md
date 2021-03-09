---
title: Обнаружение сайтов
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529311"
---
# <a name="do-site-discovery"></a><span data-ttu-id="f7c66-102">Обнаружение сайтов</span><span class="sxs-lookup"><span data-stu-id="f7c66-102">Do site discovery</span></span>

<span data-ttu-id="f7c66-103">Если в вашей организации по-прежнему используются устаревшие веб-приложения и планируется использовать режим Internet Explorer (применяемый большинством клиентов), необходимо провести дополнительное обнаружение сайтов.</span><span class="sxs-lookup"><span data-stu-id="f7c66-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="f7c66-104">**Вы уже развернули более раннюю версию Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="f7c66-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="f7c66-105">Если вы уже настроили список сайтов предприятия для работы с устаревшей версией Microsoft Edge, обнаружение сайтов почти завершено.</span><span class="sxs-lookup"><span data-stu-id="f7c66-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="f7c66-106">Вам может потребоваться лишь добавить нейтральные сайты.</span><span class="sxs-lookup"><span data-stu-id="f7c66-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="f7c66-107">Нейтральными обычно являются сайты, поддерживающие единый вход (SSO).</span><span class="sxs-lookup"><span data-stu-id="f7c66-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="f7c66-108">Если вы переходите на нейтральный сайт из Microsoft Edge, вам нужно оставаться в Microsoft Edge для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7c66-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="f7c66-109">Если вы переходите на нейтральный сайт в режиме Internet Explorer, вам нужно оставаться в режиме Internet Explorer для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f7c66-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="f7c66-110">Определите любой сайт с единым входом или другие нейтральные сайты, которые вы используете, и добавьте их в список сайтов предприятия.</span><span class="sxs-lookup"><span data-stu-id="f7c66-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="f7c66-111">**Internet Explorer является браузером по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="f7c66-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="f7c66-112">Если вы используете только Internet Explorer, возможно, вы не знаете, какие сайты были обновлены до современных веб-стандартов и какие по-прежнему требуют Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f7c66-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="f7c66-113">Вам нужно найти и добавить эти сайты в список сайтов предприятия, чтобы использовать режим Internet Explorer только для этих сайтов.</span><span class="sxs-lookup"><span data-stu-id="f7c66-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="f7c66-114">[Обнаружение сайтов предприятия](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) находит сайты, для которых может требоваться режим Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f7c66-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="f7c66-115">Эта функция может собирать данные на компьютерах под управлением Windows Internet Explorer 8 до Internet Explorer 11 в Windows 10, Windows 8.1 или Windows 7.</span><span class="sxs-lookup"><span data-stu-id="f7c66-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="f7c66-116">**Анализ данных**</span><span class="sxs-lookup"><span data-stu-id="f7c66-116">**Analyze the data**</span></span>

<span data-ttu-id="f7c66-117">После сбора данных сайтов рекомендуется выполнить четыре действия, чтобы проанализировать эти данные:</span><span class="sxs-lookup"><span data-stu-id="f7c66-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="f7c66-118">Отсортируйте данные по домену, а затем по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="f7c66-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="f7c66-119">Определите границы приложения для настройки режима Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f7c66-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="f7c66-120">Вам нужно включить все сайты и веб-элементы управления, определяющие приложение, но не нужно включать дополнительные сайты и элементы управления.</span><span class="sxs-lookup"><span data-stu-id="f7c66-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="f7c66-121">Некоторые сайты могут быть так же простыми, как *https://contoso.com/app1*, а для других может потребоваться определить несколько сайтов и страниц.</span><span class="sxs-lookup"><span data-stu-id="f7c66-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="f7c66-122">Протестируйте приложение, чтобы убедиться, что оно не работает в собственном режиме.</span><span class="sxs-lookup"><span data-stu-id="f7c66-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="f7c66-123">Многие сайты предлагают современный контент при обнаружении современного браузера и предлагают устаревший контент только при обнаружении Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f7c66-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="f7c66-124">Добавьте приложение в список сайтов предприятия, если оно не прошло тестирование.</span><span class="sxs-lookup"><span data-stu-id="f7c66-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="f7c66-125">Рекомендуется сгруппировать все сайты, составляющие приложение.</span><span class="sxs-lookup"><span data-stu-id="f7c66-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="f7c66-126">Таким образом, при обновлении приложения проще удалить весь сайт из режима Internet Explorer и начать использовать современный браузер для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="f7c66-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="f7c66-127">Закончив обнаружение сайтов и проанализировав данные, вы можете приступить к выбору стратегии канала.</span><span class="sxs-lookup"><span data-stu-id="f7c66-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

