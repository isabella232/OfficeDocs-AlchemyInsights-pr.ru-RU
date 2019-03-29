---
title: Ограничение SharePoint Online на классический режим
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953357"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="aabc0-102">Ограничение SharePoint Online на классический режим</span><span class="sxs-lookup"><span data-stu-id="aabc0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="aabc0-103">Некоторым организациям по-прежнему требуется классический режим работы.</span><span class="sxs-lookup"><span data-stu-id="aabc0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="aabc0-104">В противном случае нет планов по удалению классического режима на детализированном уровне, начиная с 1 апреля 2019 г., будет невозможно ограничить всю организацию (клиент) на классический режим для списков и библиотек.</span><span class="sxs-lookup"><span data-stu-id="aabc0-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="aabc0-105">Администратор будет иметь следующие параметры для управления отдельными списками и библиотеками в классическом режиме с использованием детализированных переключателей, которые мы предоставляем на следующих уровнях:</span><span class="sxs-lookup"><span data-stu-id="aabc0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="aabc0-106">--Site Collection--Site--List--Library</span><span class="sxs-lookup"><span data-stu-id="aabc0-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="aabc0-107">Кроме того, списки, использующие некоторые функции и настройки, которые не поддерживаются современным, по-прежнему будут автоматически переключаться на классический режим.</span><span class="sxs-lookup"><span data-stu-id="aabc0-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="aabc0-108">После 1 апреля списки и библиотеки, которые находятся в классическом режиме в результате отказа клиента, будут автоматически управляться на уровне сайта и на уровне списка.</span><span class="sxs-lookup"><span data-stu-id="aabc0-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="aabc0-109">Если вам требуется классический режим, ознакомьтесь с дополнительными сведениями здесь и инструкциями по PnP PowerShell, в которых описываются параметры и инструменты, которые можно использовать сегодня, чтобы подготовиться к удалению уровня клиента на 1 апреля.</span><span class="sxs-lookup"><span data-stu-id="aabc0-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
