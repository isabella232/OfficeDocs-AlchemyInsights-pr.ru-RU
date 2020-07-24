---
title: Exchange PowerShell и прекращение поддержки обычной проверки подлинности
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205208"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="2861a-102">Exchange PowerShell и прекращение поддержки обычной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2861a-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="2861a-103">Актуальные сведения о способе подключения к Exchange Online PowerShell без обычной проверки подлинности см. [здесь](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="2861a-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="2861a-104">Модуль PowerShell V2 не использует обычную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="2861a-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="2861a-105">Обратите внимание, что на клиентском компьютере должна быть включена обычная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="2861a-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="2861a-106">Новый модуль PowerShell версии 2 использует современную проверку подлинности с целью подключения для включения всех командлетов версии 2 на основе REST.</span><span class="sxs-lookup"><span data-stu-id="2861a-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="2861a-107">В дополнение к командлетам версии 2 он также предоставляет вам доступ к более старым командлетам PowerShell (RPS), для которых требуется создание удаленного сеанса PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2861a-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="2861a-108">Создание сеанса RPS на компьютере с Windows требует включения службы WinRM BasicAuth на клиентском компьютере, даже если модуль использует механизм современной проверки подлинности для службы.</span><span class="sxs-lookup"><span data-stu-id="2861a-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="2861a-109">Для передачи маркеров современной проверки подлинности используется конвейер обычной проверки подлинности WinRM.</span><span class="sxs-lookup"><span data-stu-id="2861a-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="2861a-110">Если на клиентском компьютере отключена обычная проверка подлинности WinRM, новые командлеты версии 2 продолжат работать (но перестанут работать более старые командлеты RPS).</span><span class="sxs-lookup"><span data-stu-id="2861a-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
