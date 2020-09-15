---
title: Проблемы с входящей миграцией машин
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676895"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="4910e-102">Проблемы с входящей миграцией машин</span><span class="sxs-lookup"><span data-stu-id="4910e-102">Issues with onboarding machines</span></span>

<span data-ttu-id="4910e-103">Могут возникнуть проблемы с входящей миграцией машин в службу MDATP.</span><span class="sxs-lookup"><span data-stu-id="4910e-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="4910e-104">Если у вас есть доступ к машине пользователя, выполните следующие шаги:</span><span class="sxs-lookup"><span data-stu-id="4910e-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="4910e-105">Скачайте средство диагностики [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="4910e-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="4910e-106">Извлеките и выполните MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="4910e-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="4910e-107">Найдите журнал диагностики в папке MDATPClientAnalyzerResult. В эту же папку загружено средство Analyzer.</span><span class="sxs-lookup"><span data-stu-id="4910e-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="4910e-108">Просмотрите файл журнала MDATPClientAnalyzer.txt, чтобы выявить проблемы с подключением или настройками прокси-сервера интернета.</span><span class="sxs-lookup"><span data-stu-id="4910e-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>