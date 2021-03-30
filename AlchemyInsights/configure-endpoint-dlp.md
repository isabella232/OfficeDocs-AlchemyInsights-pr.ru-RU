---
title: Настройка защиты от потери данных в конечной точке
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
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402449"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="24291-102">Настройка защиты от потери данных в конечной точке</span><span class="sxs-lookup"><span data-stu-id="24291-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="24291-103">Служба защиты от потери данных Microsoft Endpoint Protection позволяет расширить защиту и отслеживать конфиденциальную информацию на устройствах с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="24291-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="24291-104">После того как устройства будут интегрированы в Управление устройствами, вы сможете создавать политики защиты от потери данных.</span><span class="sxs-lookup"><span data-stu-id="24291-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="24291-105">Чтобы отслеживать действия с конфиденциальными элементами, можно использовать обозреватель действий.</span><span class="sxs-lookup"><span data-stu-id="24291-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="24291-106">Дополнительные сведения см. в статье [Интеграция устройств в управление устройствами](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="24291-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="24291-107">Чтобы приступить к работе с защитой от потери данных в конечной точке:</span><span class="sxs-lookup"><span data-stu-id="24291-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="24291-108">Убедитесь, что у вас есть соответствующая лицензия на SKU или по подписке.</span><span class="sxs-lookup"><span data-stu-id="24291-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="24291-109">Дополнительные сведения см. в статье [Лицензирование SKU и по подписке](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="24291-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="24291-110">Проверьте разрешения, необходимые для управления устройствами, доступ к странице интеграции либо включите или выключите наблюдение за устройствами.</span><span class="sxs-lookup"><span data-stu-id="24291-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="24291-111">Дополнительные сведения см. в статье [Разрешения](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="24291-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="24291-112">Внедрите устройства в средство управления устройствами, следуя соответствующей процедуре.</span><span class="sxs-lookup"><span data-stu-id="24291-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="24291-113">Если вы не видите вариант "Интеграция устройства (предварительная версия)" в **настройках** в разделе соответствия требованиям в Microsoft 365, убедитесь, что у вас есть соответствующая лицензия и разрешения, указанные выше.</span><span class="sxs-lookup"><span data-stu-id="24291-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="24291-114">Дополнительные сведения см. в статье [Интеграция устройств](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="24291-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="24291-115">Создайте политики защиты от потери данных для защиты конфиденциальных элементов.</span><span class="sxs-lookup"><span data-stu-id="24291-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="24291-116">Дополнительные сведения см. в статье [Сценарии политики защиты от потери данных в конечной точке](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="24291-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="24291-117">Дополнительные сведения о защите от потери данных можно найти в статье [Подробнее о защите от потери данных Microsoft Endpoint в Microsoft 365 (предварительная версия)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="24291-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="24291-118">**Важные шаги сбора данных, если требуется поддержка:**</span><span class="sxs-lookup"><span data-stu-id="24291-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="24291-119">Скачайте предварительную версию анализатора клиентов MDATP с сайта [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="24291-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="24291-120">Запустите средство от имени администратора из окна командной строки:</span><span class="sxs-lookup"><span data-stu-id="24291-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="24291-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="24291-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="24291-122">При появлении запроса "Введите количество минут для сбора трассировок:" введите количество минут, необходимое для выполнения сценария</span><span class="sxs-lookup"><span data-stu-id="24291-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="24291-123">Выполните сценарий</span><span class="sxs-lookup"><span data-stu-id="24291-123">Run the scenario</span></span>

<span data-ttu-id="24291-124">Получите выходной ZIP-файл для предоставления агенту службы поддержки.</span><span class="sxs-lookup"><span data-stu-id="24291-124">Collect the Zip file output to be given to the Support agent.</span></span>
