---
title: Рабочий процесс не начинается
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403756"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="3a683-102">Рабочий процесс не начинается</span><span class="sxs-lookup"><span data-stu-id="3a683-102">Workflow is not starting</span></span>

- <span data-ttu-id="3a683-103">Рабочий процесс SharePoint 2010 и SharePoint 2013 не начинается.</span><span class="sxs-lookup"><span data-stu-id="3a683-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="3a683-104">Если рабочий процесс не начинается, может возникнуть временная проблема с обслуживанием, когда пользователи могут испытывать периодические задержки с прогрессом рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="3a683-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="3a683-105">Проверьте панель [мониторинга состояния службы,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) чтобы узнать, влияет ли ваша организация на организацию.</span><span class="sxs-lookup"><span data-stu-id="3a683-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="3a683-106">Если прошло более 24 часов с тех пор, как вы впервые увидели эту проблему, зайдите в журнал билета поддержки.</span><span class="sxs-lookup"><span data-stu-id="3a683-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3a683-107">Во многих случаях мы уже работаем над решением.</span><span class="sxs-lookup"><span data-stu-id="3a683-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3a683-108">Пожалуйста, дайте нам по крайней мере 24 часа, чтобы завершить решение.</span><span class="sxs-lookup"><span data-stu-id="3a683-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="3a683-109">Рабочий процесс SharePoint 2010 отложен при запуске.</span><span class="sxs-lookup"><span data-stu-id="3a683-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="3a683-110">Это происходит, если рабочий процесс запускается большими партиями.</span><span class="sxs-lookup"><span data-stu-id="3a683-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="3a683-111">(например, при добавлении сразу нескольких элементов).</span><span class="sxs-lookup"><span data-stu-id="3a683-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="3a683-112">Рабочий процесс не предназначен для запуска в режиме реального времени, поэтому задержка — это поведение по проекту.</span><span class="sxs-lookup"><span data-stu-id="3a683-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="3a683-113">Если рабочий процесс является сложным языком разметки extensible object (XMOL), компиляция может быть медленной.</span><span class="sxs-lookup"><span data-stu-id="3a683-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="3a683-114">Проверьте [эту](https://support.microsoft.com//kb/3043697) статью.</span><span class="sxs-lookup"><span data-stu-id="3a683-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="3a683-115">Необходимо упростить рабочий процесс или изменить его с помощью типа платформы Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="3a683-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="3a683-116">Если ваша история рабочего процесса стала большой, может потребоваться очистить элементы или создать новый список истории.</span><span class="sxs-lookup"><span data-stu-id="3a683-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="3a683-117">Дополнительные сведения: [История рабочего процесса очистки](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="3a683-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="3a683-118">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="3a683-118">Related topics</span></span>
<span data-ttu-id="3a683-119">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="3a683-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3a683-120">Создание потока</span><span class="sxs-lookup"><span data-stu-id="3a683-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3a683-121">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="3a683-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
