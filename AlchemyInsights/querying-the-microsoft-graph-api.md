---
title: Запрос aPI Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950778"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="189eb-102">Запрос aPI Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="189eb-103">Этот раздел также может быть применим к разработчикам, которые по-прежнему используют API Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="189eb-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="189eb-104">Однако настоятельно рекомендуется **использовать** Microsoft Graph для всех сценариев управления каталогом, удостоверениями и доступом.</span><span class="sxs-lookup"><span data-stu-id="189eb-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="189eb-105">**Проблемы с проверкой подлинности или авторизацией**</span><span class="sxs-lookup"><span data-stu-id="189eb-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="189eb-106">Если приложению  не удается получить маркеры для вызова Microsoft Graph, выберите "Проблема с получением категории маркера доступа **(аутентификации)** Microsoft Graph", чтобы получить более подробную справку и поддержку в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="189eb-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="189eb-107">Если ваше приложение получает ошибки авторизации **401 или 403** при вызове Microsoft Graph, выберите категорию API Microsoft Graph "Получение ошибки в доступе отказано в доступе (авторизация"), чтобы получить более подробную справку и поддержку по этому разделу. </span><span class="sxs-lookup"><span data-stu-id="189eb-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="189eb-108">**Я хочу использовать Microsoft Graph, но не знаю, с чего начать**</span><span class="sxs-lookup"><span data-stu-id="189eb-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="189eb-109">Дополнительные данные о Microsoft Graph см. в:</span><span class="sxs-lookup"><span data-stu-id="189eb-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="189eb-110">Обзор Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="189eb-111">Обзор управления удостоверением и доступом в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="189eb-112">Начало создания приложений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="189eb-113">**Обозреватель Microsoft Graph:** тестирование API Microsoft Graph в клиенте или демонстрационных клиентах</span><span class="sxs-lookup"><span data-stu-id="189eb-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="189eb-114">**Я хочу использовать Microsoft Graph, но поддерживает ли он необходимые API каталогов v1.0?**</span><span class="sxs-lookup"><span data-stu-id="189eb-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="189eb-115">Microsoft Graph — это рекомендуемый API для управления каталогом, удостоверением и доступом.</span><span class="sxs-lookup"><span data-stu-id="189eb-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="189eb-116">Однако между возможными в Azure AD Graph и Microsoft Graph пробелами по-прежнему существует.</span><span class="sxs-lookup"><span data-stu-id="189eb-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="189eb-117">Просмотрите следующие статьи, в которых рассматриваются самые последние отличия, которые помогут вам в выборе:</span><span class="sxs-lookup"><span data-stu-id="189eb-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="189eb-118">Различия между типами ресурсов между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="189eb-119">Различия свойств между Azure AD Graph и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="189eb-120">Различия методов между Azure AD и Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="189eb-121">**При запросе *объекта пользователя* многие его свойства отсутствуют**</span><span class="sxs-lookup"><span data-stu-id="189eb-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="189eb-122">`GET https://graph.microsoft.com/v1.0/users`Возвращает только 11 свойств, так как Microsoft Graph автоматически  выбирает набор свойств пользователя по умолчанию для возврата.</span><span class="sxs-lookup"><span data-stu-id="189eb-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="189eb-123">Если вам нужны другие *свойства* пользователя, используйте $select, чтобы выбрать свойства, необходимые приложению.</span><span class="sxs-lookup"><span data-stu-id="189eb-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="189eb-124">Сначала попробуйте его в **microsoft Graph Explorer.**</span><span class="sxs-lookup"><span data-stu-id="189eb-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="189eb-125">**Некоторые значения свойств пользователя имеют *значение NULL,* хотя я знаю, что они установлены**</span><span class="sxs-lookup"><span data-stu-id="189eb-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="189eb-126">Наиболее вероятным объяснением является то, что приложению было предоставлено разрешение *User.ReadBasic.All.*</span><span class="sxs-lookup"><span data-stu-id="189eb-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="189eb-127">Это позволяет приложению считывать ограниченный набор свойств пользователя, возвращая все остальные свойства в качестве null, даже если они были заданной ранее.</span><span class="sxs-lookup"><span data-stu-id="189eb-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="189eb-128">Попробуйте предоставить приложению *разрешение User.Read.All.*</span><span class="sxs-lookup"><span data-stu-id="189eb-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="189eb-129">Дополнительные сведения см. в [сведениях о разрешениях пользователей Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="189eb-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="189eb-130">**У меня возникли проблемы с использованием параметров запросов OData для фильтрации данных в моих запросах**</span><span class="sxs-lookup"><span data-stu-id="189eb-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="189eb-131">Хотя Microsoft Graph поддерживает широкий спектр параметров запросов OData, многие из этих параметров не полностью поддерживаются службами каталогов (ресурсами, наследующий от *directoryObject)* в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="189eb-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="189eb-132">Те же ограничения, которые присутствуют в Azure AD Graph, по большей части сохраняются в Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="189eb-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="189eb-133">**Не поддерживается:**$count, $search и $filter значений *null* или *null*</span><span class="sxs-lookup"><span data-stu-id="189eb-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="189eb-134">**Не поддерживается:**$filter для определенных свойств (см. разделы о ресурсах, по которым можно фильтровать свойства)</span><span class="sxs-lookup"><span data-stu-id="189eb-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="189eb-135">**Не поддерживается:** одновременное разгона, фильтрация и сортировка</span><span class="sxs-lookup"><span data-stu-id="189eb-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="189eb-136">**Не поддерживается:** фильтрация по отношениям.</span><span class="sxs-lookup"><span data-stu-id="189eb-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="189eb-137">Например, найдите всех членов инженерной группы, которые находятся в Соединенном Королевстве.</span><span class="sxs-lookup"><span data-stu-id="189eb-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="189eb-138">**Частичная** поддержка: $orderby *пользователя* (только displayName и userPrincipalName) и *группы*</span><span class="sxs-lookup"><span data-stu-id="189eb-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="189eb-139">Частичная **поддержка:**$filter (поддерживает только *eq,* *startswith,* или *,* и *,* и ограниченную *любую)* поддержку, $expand (расширение связей одного объекта возвращает все связи, но расширение коллекции связей объектов ограничено)</span><span class="sxs-lookup"><span data-stu-id="189eb-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="189eb-140">Дополнительные сведения [см. в подстройке ответов с помощью параметров запроса.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="189eb-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="189eb-141">**API, который я вызываю, не работает— где можно больше тестировать?**</span><span class="sxs-lookup"><span data-stu-id="189eb-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="189eb-142">**Microsoft Graph Explorer:** тестирование API Microsoft Graph в клиенте  или демонстрационных клиентах, а также примеры запросов в проводнике Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="189eb-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="189eb-143">**При запросе данных кажется, что возвращается неполный набор данных**</span><span class="sxs-lookup"><span data-stu-id="189eb-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="189eb-144">Если вы запрашиваете коллекцию (например, *пользователей),* Microsoft Graph использует ограничения страниц на стороне сервера, чтобы результаты всегда возвращались с размером страницы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="189eb-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="189eb-145">Ваше приложение должно всегда рассчитывать на страницу с помощью коллекций, возвращаемой службой.</span><span class="sxs-lookup"><span data-stu-id="189eb-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="189eb-146">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="189eb-146">For more information, see:</span></span>

- [<span data-ttu-id="189eb-147">Лучшие методики Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="189eb-148">Разбиение данных Microsoft Graph по страницам в приложении</span><span class="sxs-lookup"><span data-stu-id="189eb-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="189eb-149">**Мое приложение работает слишком медленно и также получает регулирование. Какие улучшения можно внести?**</span><span class="sxs-lookup"><span data-stu-id="189eb-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="189eb-150">В зависимости от вашего сценария в вашем распоряжении имеется множество различных вариантов, чтобы сделать приложение более емким и в некоторых случаях менее подвержено регулированием службой (когда выполняется слишком много вызовов).</span><span class="sxs-lookup"><span data-stu-id="189eb-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="189eb-151">Дополнительные сведения см. в статьях</span><span class="sxs-lookup"><span data-stu-id="189eb-151">To learn more, see:</span></span>

- [<span data-ttu-id="189eb-152">Лучшие методики Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="189eb-153">Пакетные запросы</span><span class="sxs-lookup"><span data-stu-id="189eb-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="189eb-154">Отслеживание изменений с помощью запроса изменений</span><span class="sxs-lookup"><span data-stu-id="189eb-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="189eb-155">Получать уведомления об изменениях через веб-hooks</span><span class="sxs-lookup"><span data-stu-id="189eb-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="189eb-156">Руководство по регулированием</span><span class="sxs-lookup"><span data-stu-id="189eb-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="189eb-157">**Где можно найти дополнительные сведения об ошибках и известных проблемах?**</span><span class="sxs-lookup"><span data-stu-id="189eb-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="189eb-158">Сведения об ошибке Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="189eb-159">Известные проблемы с Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="189eb-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="189eb-160">**Где можно проверить состояние доступности и подключения службы?**</span><span class="sxs-lookup"><span data-stu-id="189eb-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="189eb-161">Доступность и подключение служб, к которые можно получить доступ через Microsoft Graph, может повлиять на общую доступность и производительность Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="189eb-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="189eb-162">Для проверки состояния службы Azure Active Directory проверьте состояние служб безопасности **и** удостоверений, перечисленных на странице [состояния Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="189eb-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="189eb-163">Для служб Office, которые внесли свой вклад в Microsoft Graph, проверьте состояние служб, перечисленных в панели мониторинга состояния служб [Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="189eb-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
