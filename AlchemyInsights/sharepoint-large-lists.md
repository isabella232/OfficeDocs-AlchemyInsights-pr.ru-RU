---
title: Крупные списки SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720146"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="4d5d3-102">Работать с большими списками и библиотеками в SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d5d3-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="4d5d3-103">Списки и библиотеки SharePoint могут содержать до 30 000 000 элементов, но если в них более 5 000 элементов, при попытке работы с ними может отобразиться пороговое значение ошибки представления списка.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="4d5d3-104">Это пороговое значение позволяет сохранить производительность службы.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="4d5d3-105">Изменить его невозможно.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-105">It can't be changed.</span></span> <span data-ttu-id="4d5d3-106">Чтобы избежать превышения этого порога:</span><span class="sxs-lookup"><span data-stu-id="4d5d3-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="4d5d3-107">**Использовать современные**</span><span class="sxs-lookup"><span data-stu-id="4d5d3-107">**Use modern**</span></span>

<span data-ttu-id="4d5d3-108">Представления, отображающие множество элементов, лучше всего подходят для современного интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="4d5d3-109">[Используйте современные возможности](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , чтобы избежать ошибок, которые могут отображаться в классическом интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="4d5d3-110">**Добавление индексов**</span><span class="sxs-lookup"><span data-stu-id="4d5d3-110">**Add indexes**</span></span>

<span data-ttu-id="4d5d3-111">При фильтрации или сортировке по столбцу, не имеющему индекса, может отобразиться сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="4d5d3-112">[Добавление индекса](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) вручную из **параметров списка** в меню Параметры, а затем **индексированные столбцы**.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="4d5d3-113">**Изменение представления списка**</span><span class="sxs-lookup"><span data-stu-id="4d5d3-113">**Edit the list view**</span></span>

<span data-ttu-id="4d5d3-114">Если при работе с большим списком возникает ошибка, [измените представление списка](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="4d5d3-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="4d5d3-115">Следующие четыре изменения будут приводить к удалению пороговых ошибок представления списка.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="4d5d3-116">Внесите все четыре изменения, чтобы удалить все ошибки.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="4d5d3-117">Если вы по-прежнему получаете ошибки, проверьте [Управление большими списками и библиотеками](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="4d5d3-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="4d5d3-118">В **None** первом случае выполните **сортировку по столбцу** , а **затем выполните сортировку по столбцу**.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="4d5d3-119">Выберите элемент **нет** из **первой группы по столбцу** , а **затем сгруппируйте по столбцу**.</span><span class="sxs-lookup"><span data-stu-id="4d5d3-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="4d5d3-120">Выберите **нет** для всех столбцов в разделе **итоги** .</span><span class="sxs-lookup"><span data-stu-id="4d5d3-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="4d5d3-121">Отмените выбор параметра все, кроме одного столбца для отображения в разделе **столбцы** .</span><span class="sxs-lookup"><span data-stu-id="4d5d3-121">Deselect all but one column for display from the **Columns** section.</span></span>

