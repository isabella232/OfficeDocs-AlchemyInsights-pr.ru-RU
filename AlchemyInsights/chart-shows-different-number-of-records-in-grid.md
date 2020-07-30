---
title: Для диаграммы отличается количество записей в сетке
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431630"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="a3891-102">Для диаграммы отличается количество записей в сетке</span><span class="sxs-lookup"><span data-stu-id="a3891-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="a3891-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="a3891-103">**Symptom**</span></span>

<span data-ttu-id="a3891-104">Если для какой-либо диаграммы на странице панели мониторинга щелкнуть "...", а затем "Просмотреть записи", откроется страница сетки, на которой можно просмотреть все записи. Иногда количество записей изменяется.</span><span class="sxs-lookup"><span data-stu-id="a3891-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="a3891-105">**Причина**</span><span class="sxs-lookup"><span data-stu-id="a3891-105">**Cause**</span></span>

<span data-ttu-id="a3891-106">Причина заключается в разнице между представлением диаграммы на исходной странице панели мониторинга и представлением диаграммы на домашней странице сетки.</span><span class="sxs-lookup"><span data-stu-id="a3891-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="a3891-107">**Решение**</span><span class="sxs-lookup"><span data-stu-id="a3891-107">**Solution**</span></span>

1. <span data-ttu-id="a3891-108">Проверьте представление на исходной странице и представление в сетке, чтобы определить, есть ли между ними разница.</span><span class="sxs-lookup"><span data-stu-id="a3891-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="a3891-109">Измените представление сетки в соответствии с исходной страницей.</span><span class="sxs-lookup"><span data-stu-id="a3891-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="a3891-110">Если не удается найти нужное представление, обычно это означает, что такое представление не включено в конструкторе приложений.</span><span class="sxs-lookup"><span data-stu-id="a3891-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="a3891-111">Перейдите в конструктор приложений для определенного приложения, выберите объект и его представления, установите флажок для представления, которое нужно включить, сохраните, опубликуйте и закройте.</span><span class="sxs-lookup"><span data-stu-id="a3891-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="a3891-112">Обновите страницу.</span><span class="sxs-lookup"><span data-stu-id="a3891-112">Refresh the page.</span></span>