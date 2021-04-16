---
title: Средство экспорта обнаруженных электронных данных
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814601"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="9ebec-102">Не можете установить или запустить средство экспорта электронных обнаружений?</span><span class="sxs-lookup"><span data-stu-id="9ebec-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="9ebec-103">Если вы не можете установить или запустить средство экспорта электронных открытий для скачивания результатов поиска, проверьте следующие вещи:</span><span class="sxs-lookup"><span data-stu-id="9ebec-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="9ebec-104">Компьютер, на который вы используете, соответствует этим предварительным требованиям:</span><span class="sxs-lookup"><span data-stu-id="9ebec-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="9ebec-105">32- или 64-разрядный выпуск Windows 7 и более поздней версии.


</span><span class="sxs-lookup"><span data-stu-id="9ebec-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="9ebec-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="9ebec-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="9ebec-107">Поддерживаемый браузер:</span><span class="sxs-lookup"><span data-stu-id="9ebec-107">A supported browser:</span></span>

  - <span data-ttu-id="9ebec-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9ebec-108">Microsoft Edge</span></span>

    <span data-ttu-id="9ebec-109">Или</span><span class="sxs-lookup"><span data-stu-id="9ebec-109">Or</span></span>

  - <span data-ttu-id="9ebec-110">Internet Explorer 10 и более поздние версии.</span><span class="sxs-lookup"><span data-stu-id="9ebec-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="9ebec-111">Другие браузеры, такие как Google Chrome и Mozilla Firefox, не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="9ebec-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="9ebec-112">Ваша организация может подключиться к конечной точке Azure, которая является **\* .blob.core.windows.net** (под диктовка представляет уникальный идентификатор для экспортной работы).</span><span class="sxs-lookup"><span data-stu-id="9ebec-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="9ebec-113">Вам назначена роль экспорта в Центре соответствия требованиям безопасности Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="9ebec-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="9ebec-114">По умолчанию эта роль назначена только группе ролей диспетчера электронных обнаружений.</span><span class="sxs-lookup"><span data-stu-id="9ebec-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="9ebec-115">См. [назначение разрешений на открытие электронной почты.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="9ebec-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="9ebec-116">Дополнительные сведения см. в [результатах поиска по экспорту контента.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="9ebec-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="9ebec-117">Если вы экспортируете более 100 000 почтовых ящиков, для скачивания результатов Экспорта: Экспорт результатов из более  [чем 100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)почтовых ящиков необходимо использовать следующие powershell.</span><span class="sxs-lookup"><span data-stu-id="9ebec-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>