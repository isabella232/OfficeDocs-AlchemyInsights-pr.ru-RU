---
title: Рабочий процесс не запускается
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738102"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="990c0-102">Рабочий процесс не запускается</span><span class="sxs-lookup"><span data-stu-id="990c0-102">Workflow is not starting</span></span>

- <span data-ttu-id="990c0-103">Рабочие процессы SharePoint 2010 и SharePoint 2013 не запускаются.</span><span class="sxs-lookup"><span data-stu-id="990c0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="990c0-104">Если рабочий процесс не запускается, возможна временная ошибка службы, из-за которой пользователи могут столкнуться с периодическими задержками, связанными с ходом выполнения рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="990c0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="990c0-105">Просмотрите [панель мониторинга работоспособности службы](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить, влияет ли ваша организация на работу.</span><span class="sxs-lookup"><span data-stu-id="990c0-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="990c0-106">Если вы пропустили эту ошибку более 24 часов, запишите запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="990c0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="990c0-107">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="990c0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="990c0-108">Отправьте нам по крайней мере 24 часа для завершения решения.</span><span class="sxs-lookup"><span data-stu-id="990c0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="990c0-109">Рабочие процессы SharePoint 2010, задержанные при запуске.</span><span class="sxs-lookup"><span data-stu-id="990c0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="990c0-110">Это происходит, если рабочий процесс запускается в больших пакетах.</span><span class="sxs-lookup"><span data-stu-id="990c0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="990c0-111">(например, при одновременном добавлении нескольких элементов).</span><span class="sxs-lookup"><span data-stu-id="990c0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="990c0-112">Рабочие процессы не предназначены для работы в режиме реального времени, поэтому задержка связана с поведением по проектированию.</span><span class="sxs-lookup"><span data-stu-id="990c0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="990c0-113">Если рабочий процесс является сложным языковым языком разметки объектов (КСМОЛ), компиляция может выполняться медленно.</span><span class="sxs-lookup"><span data-stu-id="990c0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="990c0-114">Обратитесь к [этой](https://support.microsoft.com//kb/3043697) статье.</span><span class="sxs-lookup"><span data-stu-id="990c0-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="990c0-115">Необходимо упростить рабочий процесс или изменить его с помощью типа платформы рабочих процессов Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="990c0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="990c0-116">Если размер журнала рабочего процесса увеличился, можно удалить элементы или создать новый список журналов.</span><span class="sxs-lookup"><span data-stu-id="990c0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="990c0-117">Дополнительные сведения: [Очистка журнала рабочих процессов](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="990c0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="990c0-118">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="990c0-118">Related topics</span></span>
<span data-ttu-id="990c0-119">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="990c0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="990c0-120">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="990c0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="990c0-121">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="990c0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


