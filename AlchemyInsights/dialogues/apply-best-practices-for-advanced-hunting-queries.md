---
title: Применение передовых методов для расширенных запросов на охоту
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568719"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="2edab-102">Применение передовых методов для расширенных запросов на охоту</span><span class="sxs-lookup"><span data-stu-id="2edab-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="2edab-103">Чтобы получить результаты быстрее и избежать периодов времени при работе со сложными запросами, применяем эти методы:</span><span class="sxs-lookup"><span data-stu-id="2edab-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="2edab-104">При попытке новых запросов всегда используйте ограничение, чтобы избежать получения очень больших наборов результатов.</span><span class="sxs-lookup"><span data-stu-id="2edab-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="2edab-105">Кроме того, `count` используйте для первоначальной оценки размера набора результатов.</span><span class="sxs-lookup"><span data-stu-id="2edab-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="2edab-106">Временные фильтры рекомендуется применять в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="2edab-106">Use time filters first.</span></span> <span data-ttu-id="2edab-107">В идеале ограничьте запросы семи днями.</span><span class="sxs-lookup"><span data-stu-id="2edab-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="2edab-108">В начале запроса сразу после фильтра времени добавьте фильтры, которые, как ожидается, удалят большую часть данных.</span><span class="sxs-lookup"><span data-stu-id="2edab-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="2edab-109">При поиске полных маркеров используйте `has` оператора, а не `contains` .</span><span class="sxs-lookup"><span data-stu-id="2edab-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="2edab-110">Запустите поиск в определенном столбце, а не во всех столбцах.</span><span class="sxs-lookup"><span data-stu-id="2edab-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="2edab-111">При присоединении к таблицам сначала укажите таблицу с большим количеством строк.</span><span class="sxs-lookup"><span data-stu-id="2edab-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="2edab-112">`project` только необходимые столбцы из таблиц, к которые вы присоединились.</span><span class="sxs-lookup"><span data-stu-id="2edab-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="2edab-113">Дополнительные данные см. в дополнительных практических действиях по [запросу расширенных запросов.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="2edab-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
