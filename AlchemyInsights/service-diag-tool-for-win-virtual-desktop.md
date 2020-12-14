---
title: Средство диагностики служб для виртуального рабочего стола Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665827"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="f26d5-102">Средство диагностики служб для виртуального рабочего стола Windows</span><span class="sxs-lookup"><span data-stu-id="f26d5-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="f26d5-103">Виртуальный рабочий стол Windows (WVD) предлагает средство диагностики, которое позволяет администраторам выявлять ошибки с помощью одного интерфейса.</span><span class="sxs-lookup"><span data-stu-id="f26d5-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="f26d5-104">Это средство записывает в журнал сведения, связанные с диагностикой, каждый раз, когда WVD используется кем-то, кому назначена роль WVD.</span><span class="sxs-lookup"><span data-stu-id="f26d5-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="f26d5-105">Каждый журнал содержит сведения о роли WVD, которая участвует в действии, сообщения об ошибках, которые отображаются во время сеанса, а также сведения о клиенте и пользователе.</span><span class="sxs-lookup"><span data-stu-id="f26d5-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="f26d5-106">Azure Log Analytics можно настроить для записи журнала действий, созданного средством диагностики.</span><span class="sxs-lookup"><span data-stu-id="f26d5-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="f26d5-107">Вот как это сделать:</span><span class="sxs-lookup"><span data-stu-id="f26d5-107">Here's how:</span></span>

1. <span data-ttu-id="f26d5-108">Создайте рабочее пространство Log Analytics с помощью портала [Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="f26d5-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="f26d5-109">[Подключите компьютеры с Windows к Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="f26d5-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="f26d5-110">Получите ИД рабочей области и первичный ключ рабочей области.</span><span class="sxs-lookup"><span data-stu-id="f26d5-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="f26d5-111">Эти сведения необходимы мастеру настройки, чтобы правильно настроить агент и убедиться, что он может взаимодействовать с Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="f26d5-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="f26d5-112">[Push-диагностические данные в рабочей области.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="f26d5-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="f26d5-113">Диагностические данные из клиента WVD можно вывести в аналитику журналов для своей рабочей области.</span><span class="sxs-lookup"><span data-stu-id="f26d5-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="f26d5-114">[Выявлять и диагностировать внутренние](https://go.microsoft.com/fwlink/?linkid=2128338) или внешние проблемы по отношению к WVD.</span><span class="sxs-lookup"><span data-stu-id="f26d5-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="f26d5-115">Дополнительные данные о настройке средства диагностики служб для WVD см. в средстве ["Use Log Analytics for the diagnostics feature".](https://go.microsoft.com/fwlink/?linkid=2128084)</span><span class="sxs-lookup"><span data-stu-id="f26d5-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
