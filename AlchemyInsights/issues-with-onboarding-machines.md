---
title: Проблемы с подключением компьютеров к Microsoft Defender для конечной точки
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901580"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="3d30b-102">Проблемы с подключением компьютеров к Microsoft Defender для конечной точки</span><span class="sxs-lookup"><span data-stu-id="3d30b-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="3d30b-103">У вас могут возникнуть проблемы с подключением компьютеров к службе MDE.</span><span class="sxs-lookup"><span data-stu-id="3d30b-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="3d30b-104">Если у вас есть доступ к компьютеру пользователя, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3d30b-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="3d30b-105">Скачайте последнюю предварительную версию средства диагностики [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="3d30b-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="3d30b-106">Щелкните правой кнопкой **MDEClientAnalyzer.cmd** и выберите "Запуск от имени администратора".</span><span class="sxs-lookup"><span data-stu-id="3d30b-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="3d30b-107">Следуйте рекомендациям, предлагаемым в **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="3d30b-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="3d30b-108">Более подробные журналы можно просмотреть в созданной вложенной папке с именем **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="3d30b-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="3d30b-109">Если требуется дополнительное руководство, обратитесь в [службу поддержки Microsoft Defender для конечной точки](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) и предоставьте итоговый файл MDEClientAnalyzerResult.zip для анализа.</span><span class="sxs-lookup"><span data-stu-id="3d30b-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
