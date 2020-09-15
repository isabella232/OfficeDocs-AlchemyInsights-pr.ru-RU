---
title: Средство экспорта обнаруженных электронных данных
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711108"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="ab155-102">Не удается установить или запустить средство экспорта обнаружения электронных данных?</span><span class="sxs-lookup"><span data-stu-id="ab155-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="ab155-103">Если вы не можете установить или запустить средство экспорта eDiscovery для загрузки результатов поиска, проверьте следующие моменты.</span><span class="sxs-lookup"><span data-stu-id="ab155-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="ab155-104">Компьютер, который вы используете, соответствует этим предварительным требованиям:</span><span class="sxs-lookup"><span data-stu-id="ab155-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="ab155-105">32- или 64-разрядный выпуск Windows 7 и более поздней версии.


</span><span class="sxs-lookup"><span data-stu-id="ab155-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="ab155-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="ab155-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="ab155-107">Поддерживаемый браузер:</span><span class="sxs-lookup"><span data-stu-id="ab155-107">A supported browser:</span></span>

  - <span data-ttu-id="ab155-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ab155-108">Microsoft Edge</span></span>

    <span data-ttu-id="ab155-109">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="ab155-109">Or</span></span>

  - <span data-ttu-id="ab155-110">Internet Explorer 10 и более поздние версии.</span><span class="sxs-lookup"><span data-stu-id="ab155-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="ab155-111">Другие браузеры, такие как Google Chrome и Mozilla Firefox, не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ab155-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="ab155-112">Ваша организация может подключаться к конечной точке в Azure, т \*\* \* . е. BLOB.Core.Windows.NET\*\* (подстановочный знак представляет уникальный идентификатор задания экспорта).</span><span class="sxs-lookup"><span data-stu-id="ab155-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="ab155-113">Вы назначили роль экспорт в центре безопасности Майкрософт 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="ab155-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="ab155-114">По умолчанию эта роль назначается только группе ролей диспетчера обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="ab155-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="ab155-115">См. [Назначение разрешений на обнаружение электронных](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)данных.</span><span class="sxs-lookup"><span data-stu-id="ab155-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="ab155-116">Дополнительные сведения можно найти в статье [Экспорт результатов поиска контента](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="ab155-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>
  