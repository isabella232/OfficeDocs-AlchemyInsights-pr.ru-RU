---
title: Проблемы с производительностью Microsoft Defender для конечной точки в Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783431"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="1ed2c-102">Проблемы с производительностью Microsoft Defender для конечной точки в Linux</span><span class="sxs-lookup"><span data-stu-id="1ed2c-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="1ed2c-103">В этой статье описаны действия по выявлению проблем с производительностью Microsoft Defender для конечной точки в Linux.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="1ed2c-104">Сначала необходимо убедиться, что проблема, с которой вы столкнулись, устранена в [последней версии](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="1ed2c-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="1ed2c-105">Прежде чем приступить к исследованию, см. статью [Устранение неполадок с производительностью Microsoft Defender для конечной точки в Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="1ed2c-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="1ed2c-106">Исключения</span><span class="sxs-lookup"><span data-stu-id="1ed2c-106">Exclusions</span></span>

<span data-ttu-id="1ed2c-107">Исключения могут помочь устранить проблемы с производительностью.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="1ed2c-108">Прежде чем приступить к работе, просмотрите исключения, чтобы выявить и задокументировать любой дополнительный риск.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="1ed2c-109">Дополнительные сведения см. в статье [Настройка и проверка исключений Microsoft Defender для конечной точки в Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="1ed2c-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="1ed2c-110">Если необходимо исключить несколько файлов и папок, которые находятся в одной точке подключения, рекомендуется исключить точку подключения.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="1ed2c-111">Начиная с февральского выпуска 101.22.80, вы сможете исключить всю точку подключения.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="1ed2c-112">Например, если /mnt/backup является точкой подключения, вы можете добавить /mnt/backup в список исключений, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="1ed2c-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="1ed2c-113">**Примечание**. Добавление исключений увеличивает риск неполного обнаружения вредоносных программ, поэтому их следует применять с осторожностью.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="1ed2c-114">Нужна помощь?</span><span class="sxs-lookup"><span data-stu-id="1ed2c-114">Need Help?</span></span>

<span data-ttu-id="1ed2c-115">Чтобы мы могли вам оказать более эффективную помощь, соберите диагностические данные перед обращением в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="1ed2c-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
