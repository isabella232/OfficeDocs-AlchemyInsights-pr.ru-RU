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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657942"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="77bd5-102">Настройка защиты от потери данных в конечной точке</span><span class="sxs-lookup"><span data-stu-id="77bd5-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="77bd5-103">Служба защиты от потери данных Microsoft Endpoint Protection позволяет расширить защиту и отслеживать конфиденциальную информацию на устройствах с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="77bd5-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="77bd5-104">После того как устройства будут интегрированы в Управление устройствами, вы сможете создавать политики защиты от потери данных.</span><span class="sxs-lookup"><span data-stu-id="77bd5-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="77bd5-105">Чтобы отслеживать действия с конфиденциальными элементами, можно использовать обозреватель действий.</span><span class="sxs-lookup"><span data-stu-id="77bd5-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="77bd5-106">Дополнительные сведения см. в статье [Интеграция устройств в управление устройствами](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="77bd5-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="77bd5-107">Чтобы приступить к работе с защитой от потери данных в конечной точке:</span><span class="sxs-lookup"><span data-stu-id="77bd5-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="77bd5-108">Убедитесь, что у вас есть соответствующая лицензия на SKU или по подписке.</span><span class="sxs-lookup"><span data-stu-id="77bd5-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="77bd5-109">Дополнительные сведения см. в статье [Лицензирование SKU и по подписке](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="77bd5-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="77bd5-p103">Проверьте разрешения, необходимые для управления устройствами, доступ к странице интеграции либо включите или выключите наблюдение за устройствами. Чтобы узнать больше, см. [Разрешения](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="77bd5-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="77bd5-112">Внедрите устройства в средство управления устройствами, следуя соответствующей процедуре.</span><span class="sxs-lookup"><span data-stu-id="77bd5-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="77bd5-113">Дополнительные сведения см. в статье [Интеграция устройств](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="77bd5-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="77bd5-114">Создайте политики защиты от потери данных для защиты конфиденциальных элементов.</span><span class="sxs-lookup"><span data-stu-id="77bd5-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="77bd5-115">Дополнительные сведения см. в статье [Сценарии политики защиты от потери данных в конечной точке](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="77bd5-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="77bd5-116">Дополнительные сведения о защите от потери данных можно найти в статье [Подробнее о защите от потери данных Microsoft Endpoint в Microsoft 365 (предварительная версия)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="77bd5-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="77bd5-117">**Важные шаги сбора данных, если требуется поддержка:**</span><span class="sxs-lookup"><span data-stu-id="77bd5-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="77bd5-118">Скачайте [предварительную версию анализатора клиентов MDATP](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="77bd5-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="77bd5-119">Запустите средство от имени администратора из окна командной строки:</span><span class="sxs-lookup"><span data-stu-id="77bd5-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="77bd5-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="77bd5-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="77bd5-121">При появлении запроса **Введите количество минут для сбора трассировок:** введите количество минут, необходимое для выполнения сценария.</span><span class="sxs-lookup"><span data-stu-id="77bd5-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="77bd5-122">Выполните сценарий</span><span class="sxs-lookup"><span data-stu-id="77bd5-122">Run the scenario.</span></span>

<span data-ttu-id="77bd5-123">Получите выходной ZIP-файл для предоставления агенту службы поддержки.</span><span class="sxs-lookup"><span data-stu-id="77bd5-123">Collect the Zip file output to give to the Support agent.</span></span>
