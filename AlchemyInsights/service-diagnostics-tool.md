---
title: Средство диагностики служб для Виртуального рабочего стола Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590299"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="fca97-102">Средство диагностики служб для Виртуального рабочего стола Windows</span><span class="sxs-lookup"><span data-stu-id="fca97-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="fca97-103">Виртуальный рабочий стол Windows (WVD) предоставляет средство диагностики, позволяющее администраторам выявлять ошибки в едином интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="fca97-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="fca97-104">Это средство регистрирует диагностические данные, каждый раз, когда WVD используется пользователем, которому назначена роль WVD.</span><span class="sxs-lookup"><span data-stu-id="fca97-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="fca97-105">Каждый журнал содержит сведения о роли WVD, связанной с определенными действиями, сообщения об ошибках, отображающиеся во время сеанса, а также сведения о клиенте и пользователе.</span><span class="sxs-lookup"><span data-stu-id="fca97-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="fca97-106">Чтобы настроить службу аналитики журналов Azure для записи журнала действий, созданного средством диагностики, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="fca97-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="fca97-107">Создайте рабочую область службы аналитики журналов с помощью [портала Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="fca97-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="fca97-108">[Подключите компьютеры с Windows к Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="fca97-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="fca97-109">Получите идентификатор и первичный ключ рабочей области.</span><span class="sxs-lookup"><span data-stu-id="fca97-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="fca97-110">Эти данные необходимы мастеру установки, чтобы правильно настроить агент и обеспечить его связь с Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="fca97-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="fca97-111">[Перенесите диагностические данные в рабочую область](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="fca97-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="fca97-112">Вы можете перенести диагностические данные из клиента WVD в службу аналитики журналов для вашей рабочей области.</span><span class="sxs-lookup"><span data-stu-id="fca97-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="fca97-113">[Выполните поиск и диагностику](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) проблем, которые являются внутренними или внешними по отношению к WVD.</span><span class="sxs-lookup"><span data-stu-id="fca97-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="fca97-114">Дополнительные сведения о настройке средства диагностики служб для WVD см. в статье "Использование службы аналитики журналов в целях диагностики".</span><span class="sxs-lookup"><span data-stu-id="fca97-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>