---
title: Проблемы с входящей миграцией машин
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139057"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="8fc85-102">Проблемы с входящей миграцией машин</span><span class="sxs-lookup"><span data-stu-id="8fc85-102">Issues with onboarding machines</span></span>

<span data-ttu-id="8fc85-103">Могут возникнуть проблемы с входящей миграцией машин в службу MDATP.</span><span class="sxs-lookup"><span data-stu-id="8fc85-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="8fc85-104">Если у вас есть доступ к машине пользователя, выполните следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="8fc85-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="8fc85-105">Скачайте средство диагностики [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="8fc85-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="8fc85-106">Извлеките и выполните MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="8fc85-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="8fc85-107">Найдите журнал диагностики в папке MDATPClientAnalyzerResult. В эту же папку загружено средство Analyzer.</span><span class="sxs-lookup"><span data-stu-id="8fc85-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="8fc85-108">Просмотрите файл журнала MDATPClientAnalyzer.txt, чтобы выявить проблемы с подключением или настройками прокси-сервера интернета.</span><span class="sxs-lookup"><span data-stu-id="8fc85-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>