---
title: Выявление проблем Виртуального рабочего стола Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590298"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="4a4f8-102">Выявление проблем Виртуального рабочего стола Windows</span><span class="sxs-lookup"><span data-stu-id="4a4f8-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="4a4f8-103">Служба диагностики Виртуального рабочего стола Windows использует только один командлет PowerShell, но содержит множество дополнительных параметров, позволяющих сузить круг проблем и изолировать их.</span><span class="sxs-lookup"><span data-stu-id="4a4f8-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="4a4f8-104">Чтобы начать, выполните следующее.</span><span class="sxs-lookup"><span data-stu-id="4a4f8-104">To get started:</span></span> 

1. <span data-ttu-id="4a4f8-105">Скачайте и импортируйте модуль PowerShell для Виртуального рабочего стола Windows.</span><span class="sxs-lookup"><span data-stu-id="4a4f8-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="4a4f8-106">Дополнительные сведения см. в статье [Командлеты Виртуального рабочего стола Windows для Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="4a4f8-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="4a4f8-107">Запустите следующий командлет, чтобы войти в свою учетную запись:</span><span class="sxs-lookup"><span data-stu-id="4a4f8-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="4a4f8-108">Пример: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="4a4f8-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="4a4f8-109">**ПРИМЕЧАНИЕ.** Все запросы, использующие PowerShell, должны включать параметры -UserName или -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="4a4f8-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="4a4f8-110">Дополнительные сведения о возможностях мониторинга см. в статье [Использование службы аналитики журналов в целях диагностики](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="4a4f8-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="4a4f8-111">Чтобы отфильтровать диагностические действия по пользователям, выполните следующий командлет:</span><span class="sxs-lookup"><span data-stu-id="4a4f8-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="4a4f8-112">Пример: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="4a4f8-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="4a4f8-113">Для диагностики проблем можно использовать имеющийся список фильтров.</span><span class="sxs-lookup"><span data-stu-id="4a4f8-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="4a4f8-114">Дополнительные сведения о диагностике проблем см. в статье [Выявление и диагностика проблем Виртуального рабочего стола Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="4a4f8-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="4a4f8-115">Дополнительные сведения о распространенных ошибках см. в разделе [Распространенные сценарии ошибок](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="4a4f8-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
