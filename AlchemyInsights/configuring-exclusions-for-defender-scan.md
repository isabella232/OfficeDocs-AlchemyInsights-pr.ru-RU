---
title: Настройка исключений для сканирования в защитнике Microsoft Defender
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768488"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="6ec0f-102">Настройка исключений для сканирования в защитнике Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="6ec0f-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="6ec0f-103">В общем случае можно исключить файлы с определенными расширениями и определенные папки из сканирования Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="6ec0f-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="6ec0f-104">Кроме того, можно настроить исключения для файлов, открытых определенными процессами.</span><span class="sxs-lookup"><span data-stu-id="6ec0f-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="6ec0f-105">Дополнительные сведения см. в статье [Настройка и проверка исключений с учетом расширения файла и расположения папки](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) и [Настройка исключений для файлов, открытых процессами](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="6ec0f-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="6ec0f-106">Сведения о том, как настроить исключения для  **Windows Server 2016 и 2019**, см. в статье [Исключения антивирусной программы Microsoft Defender на сервере Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="6ec0f-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="6ec0f-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="6ec0f-107">**Mac**</span></span>

<span data-ttu-id="6ec0f-108">Подробные сведения о поддерживаемых типах исключений и настройке списка исключений для Mac см. в статьях [Поддерживаемые типы исключений](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) и [Как настроить список исключений](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="6ec0f-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="6ec0f-109">**Примечание.** Можно также проверять списки исключений с помощью тестового файла EICAR.</span><span class="sxs-lookup"><span data-stu-id="6ec0f-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="6ec0f-110">Дополнительную информацию см. в статье [Проверка списков исключений с помощью тестового файла EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="6ec0f-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="6ec0f-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="6ec0f-111">**Linux**</span></span>

<span data-ttu-id="6ec0f-112">Подробные сведения о поддерживаемых типах исключений и настройке списка исключений для Linux см. в статьях [Поддерживаемые типы исключений](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) и [Как настроить список исключений Microsoft Defender ATP для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="6ec0f-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="6ec0f-113">**Примечание.** Можно также проверять списки исключений с помощью тестового файла EICAR.</span><span class="sxs-lookup"><span data-stu-id="6ec0f-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="6ec0f-114">Дополнительную информацию см. в статье [Проверка списков исключений с помощью тестового файла EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="6ec0f-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 