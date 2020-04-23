---
title: Ограничение SharePoint Online на классический режим
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742482"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="6f75b-102">Ограничение SharePoint Online на классический режим</span><span class="sxs-lookup"><span data-stu-id="6f75b-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="6f75b-103">Некоторым организациям по-прежнему требуется классический режим работы.</span><span class="sxs-lookup"><span data-stu-id="6f75b-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="6f75b-104">В противном случае нет планов по удалению классического режима на детализированном уровне, поэтому больше невозможно ограничить всю организацию (клиент) на классический режим для списков и библиотек.</span><span class="sxs-lookup"><span data-stu-id="6f75b-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="6f75b-105">Администратор будет иметь следующие параметры для управления отдельными списками и библиотеками в классическом режиме с использованием детализированных переключателей, которые мы предоставляем на следующих уровнях:</span><span class="sxs-lookup"><span data-stu-id="6f75b-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="6f75b-106">семейство веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="6f75b-106">site collection</span></span>
- <span data-ttu-id="6f75b-107">site</span><span class="sxs-lookup"><span data-stu-id="6f75b-107">site</span></span>
- <span data-ttu-id="6f75b-108">список</span><span class="sxs-lookup"><span data-stu-id="6f75b-108">list</span></span>
- <span data-ttu-id="6f75b-109">см</span><span class="sxs-lookup"><span data-stu-id="6f75b-109">library</span></span>

<span data-ttu-id="6f75b-110">Кроме того, списки, использующие некоторые функции и настройки, которые не поддерживаются современным, по-прежнему будут автоматически переключаться на классический режим.</span><span class="sxs-lookup"><span data-stu-id="6f75b-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="6f75b-111">Начиная с 1 апреля 2019 г., процесс отключения отказа от использования современного списка и библиотек на уровне клиента будет начинаться и продолжаться до 31 мая 2019.</span><span class="sxs-lookup"><span data-stu-id="6f75b-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="6f75b-112">Списки и библиотеки, которые находятся в классическом режиме в результате отказа клиента, автоматически перемещаются на современные.</span><span class="sxs-lookup"><span data-stu-id="6f75b-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="6f75b-113">Если вам нужен классический режим, [Ознакомьтесь с дополнительными сведениями](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) и инструкциями по PnP PowerShell, в которых описываются параметры и инструменты [, которые можно](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) использовать сегодня для использования классического режима работы.</span><span class="sxs-lookup"><span data-stu-id="6f75b-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
