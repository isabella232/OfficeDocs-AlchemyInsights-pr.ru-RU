---
title: События календаря отсутствуют или не обновляются
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819983"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="178d4-102">События календаря отсутствуют или не обновляются</span><span class="sxs-lookup"><span data-stu-id="178d4-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="178d4-103">Если элементы календаря отсутствуют или не обновляются, сначала проверьте количество элементов в свойствах папки "Календарь" в Outlook:</span><span class="sxs-lookup"><span data-stu-id="178d4-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="178d4-104">Щелкните правой кнопкой мыши папку **Календарь** затронутого пользователя и выберите **Свойства**.</span><span class="sxs-lookup"><span data-stu-id="178d4-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="178d4-105">Выберите вкладку **Синхронизация**.</span><span class="sxs-lookup"><span data-stu-id="178d4-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="178d4-106">Если количество элементов в папке на сервере и автономной папке не совпадает:</span><span class="sxs-lookup"><span data-stu-id="178d4-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="178d4-107">Выделите папку **Календарь**.</span><span class="sxs-lookup"><span data-stu-id="178d4-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="178d4-108">Перейдите на вкладку **Отправка**/**получение** и нажмите **Обновить папку**.</span><span class="sxs-lookup"><span data-stu-id="178d4-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="178d4-109">Если календарь по-прежнему не обновляется или события отсутствуют, скачайте средство проверки календаря для Outlook из [Центра загрузки Майкрософт](https://www.microsoft.com/download/details.aspx?id=28786).</span><span class="sxs-lookup"><span data-stu-id="178d4-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="178d4-110">Проверьте, содержится ли в папке календаря более 5000 элементов, так как это может вызывать проблемы, например собрания календаря не обновляются или возникают ошибки собраний.</span><span class="sxs-lookup"><span data-stu-id="178d4-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="178d4-111">Дополнительные сведения см. в статье [Проблемы с производительностью Outlook при слишком большом количестве элементов или папок в кэшированном режиме файла OST или PST](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span><span class="sxs-lookup"><span data-stu-id="178d4-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>