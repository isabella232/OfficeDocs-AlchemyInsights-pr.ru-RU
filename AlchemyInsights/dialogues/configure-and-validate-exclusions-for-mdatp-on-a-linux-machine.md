---
title: Настройка и проверка исключений для MDATP на компьютере Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568718"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="2f55f-102">Настройка и проверка исключений для MDATP на компьютере Linux</span><span class="sxs-lookup"><span data-stu-id="2f55f-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="2f55f-103">Некоторые файлы, папки, процессы и файлы, открытые процессом, можно исключить из сканирования MDATP.</span><span class="sxs-lookup"><span data-stu-id="2f55f-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="2f55f-104">Исключения помогают предотвратить неправильное обнаружение программного обеспечения и файлов, уникальных или настраиваемых для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="2f55f-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="2f55f-105">Исключения также помогают устранить проблемы производительности, вызванные MDATP.</span><span class="sxs-lookup"><span data-stu-id="2f55f-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="2f55f-106">Дополнительные данные см. в дополнительных подробной информации о настройке и [проверке исключений для MDATP для Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="2f55f-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2f55f-107">Исключения, описанные в этой статье, не применяются к другим возможностям MDATP для Linux, включая обнаружение конечных точек и ответ (EDR).</span><span class="sxs-lookup"><span data-stu-id="2f55f-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="2f55f-108">Файлы, которые вы исключаете с помощью методов, описанных в этой статье, по-прежнему могут вызывать оповещения EDR и другие возможности обнаружения.</span><span class="sxs-lookup"><span data-stu-id="2f55f-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
