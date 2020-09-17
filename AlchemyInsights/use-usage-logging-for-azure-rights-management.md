---
title: Использование журнала использования защиты для Azure Rights Management
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: f1483e177ec6fcdd39d0aae481d3b329b11577d4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796805"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="e55d5-102">Использование журнала использования защиты для Azure Rights Management</span><span class="sxs-lookup"><span data-stu-id="e55d5-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="e55d5-103">По умолчанию ведение журнала использования включено для всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="e55d5-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="e55d5-104">Журналы записываются в хранилище Azure как последовательность больших двоичных объектов для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="e55d5-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="e55d5-105">После выполнения действия защиты большинство журналов будет доступно приблизительно через 15 минут.</span><span class="sxs-lookup"><span data-stu-id="e55d5-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="e55d5-106">Журналы использования защиты можно использовать в следующих целях:</span><span class="sxs-lookup"><span data-stu-id="e55d5-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="e55d5-107">для бизнес-аналитики;</span><span class="sxs-lookup"><span data-stu-id="e55d5-107">Analyze business insights</span></span>

- <span data-ttu-id="e55d5-108">для того, чтобы следить за нарушениями;</span><span class="sxs-lookup"><span data-stu-id="e55d5-108">Monitor for abuse</span></span>

- <span data-ttu-id="e55d5-109">для проведения судебного анализа.</span><span class="sxs-lookup"><span data-stu-id="e55d5-109">Perform forensic analysis</span></span>

<span data-ttu-id="e55d5-110">Дополнительные сведения см. в статье [Ведение журнала и анализ использования защиты Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="e55d5-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="e55d5-111">Сведения о ведении журналов использования клиентов см. в статье [Руководство для администратора: файлы клиента Azure Information Protection и ведение журнала использования для клиента](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="e55d5-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="e55d5-112">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="e55d5-112">For additional information, see:</span></span>

- <span data-ttu-id="e55d5-113">[Требования Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="e55d5-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="e55d5-114">[Руководство: настройка параметров политики Azure Information Protection и создание новой метки](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="e55d5-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>