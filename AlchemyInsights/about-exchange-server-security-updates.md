---
title: Обновления Exchange Server безопасности
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449096"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="84510-102">Обновления Exchange Server безопасности</span><span class="sxs-lookup"><span data-stu-id="84510-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="84510-103">Корпорация Майкрософт выпустила ряд критически важных обновлений безопасности для Exchange Server локальной службы.</span><span class="sxs-lookup"><span data-stu-id="84510-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="84510-104">Затронутые версии серверов — это уровни обновления Exchange Server 2010, 2013, 2016 и 2019 годов.</span><span class="sxs-lookup"><span data-stu-id="84510-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="84510-105">Exchange Online не влияет, но если у вас есть некоторые локально серверы Exchange из-за гибридной конфигурации, они потенциально уязвимы.</span><span class="sxs-lookup"><span data-stu-id="84510-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="84510-106">Для обновления локального сервера необходимо будет запускать по крайней мере следующие версии Exchange:</span><span class="sxs-lookup"><span data-stu-id="84510-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="84510-107">Exchange 2010 Пакет обновления 3</span><span class="sxs-lookup"><span data-stu-id="84510-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="84510-108">Exchange Server 2013 cu 23</span><span class="sxs-lookup"><span data-stu-id="84510-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="84510-109">Exchange Server 2016 cu 19 или CU 18</span><span class="sxs-lookup"><span data-stu-id="84510-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="84510-110">Exchange Server 2019 cu 8 или CU 7</span><span class="sxs-lookup"><span data-stu-id="84510-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="84510-111">См. в следующем объявлении о расположении исправлений: [Released: March 2021 Exchange Server обновления безопасности](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="84510-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="84510-112">**Важные примечания.**</span><span class="sxs-lookup"><span data-stu-id="84510-112">**Important notes:**</span></span>

<span data-ttu-id="84510-113">Установка обновлений не будет работать, если на локальном сервере не запущены необходимые версии Exchange, как по вышеуказанном списку.</span><span class="sxs-lookup"><span data-stu-id="84510-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="84510-114">При установке обновлений вручную ознакомьтесь с разделом "Известные проблемы" обновления статей КБ для получения важных сведений.</span><span class="sxs-lookup"><span data-stu-id="84510-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="84510-115">Обновления безопасности должны запускаться с повышенной подсказки CMD/PowerShell!</span><span class="sxs-lookup"><span data-stu-id="84510-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
