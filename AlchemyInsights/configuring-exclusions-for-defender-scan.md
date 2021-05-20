---
title: Настройка исключений для сканирования в ATP в Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543698"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="1e84d-102">Настройка исключений для сканирования в ATP в Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="1e84d-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="1e84d-103">В общем случае можно исключить файлы с определенными расширениями и определенные папки из сканирования ATP в Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="1e84d-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="1e84d-104">Кроме того, можно настроить исключения для файлов, открытых определенными процессами.</span><span class="sxs-lookup"><span data-stu-id="1e84d-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="1e84d-105">Дополнительные сведения см. в статье [Настройка и проверка исключений с учетом расширения файла и расположения папки](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) и [Настройка исключений для файлов, открытых процессами](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="1e84d-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="1e84d-106">Сведения о том, как настроить исключения для **Windows Server 2016 и 2019**, см. в статье [Исключения антивирусной программы Microsoft Defender на сервере Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="1e84d-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="1e84d-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="1e84d-107">**Mac**</span></span>

<span data-ttu-id="1e84d-108">Подробные сведения о поддерживаемых типах исключений и настройке списка исключений для Mac см. в статьях [Поддерживаемые типы исключений](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) и [Как настроить список исключений](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="1e84d-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="1e84d-109">**Примечание.** Можно также проверять списки исключений с помощью тестового файла EICAR.</span><span class="sxs-lookup"><span data-stu-id="1e84d-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="1e84d-110">Дополнительную информацию см. в статье [Проверка списков исключений с помощью тестового файла EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="1e84d-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="1e84d-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="1e84d-111">**Linux**</span></span>

<span data-ttu-id="1e84d-112">Подробные сведения о поддерживаемых типах исключений и настройке списка исключений для Linux см. в статьях [Поддерживаемые типы исключений](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) и [Как настроить список исключений Microsoft Defender ATP для Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="1e84d-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="1e84d-113">**Примечание.** Можно также проверять списки исключений с помощью тестового файла EICAR.</span><span class="sxs-lookup"><span data-stu-id="1e84d-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="1e84d-114">Дополнительную информацию см. в статье [Проверка списков исключений с помощью тестового файла EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="1e84d-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 