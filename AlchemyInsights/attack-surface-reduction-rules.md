---
title: Правила сокращения направлений атак
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651503"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="be4ed-102">Правила сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="be4ed-102">Attack surface reduction rules</span></span>

<span data-ttu-id="be4ed-103">Исключение файлов или папок может значительно снизить защиту, предоставляемую правилами сокращения направлений атак.</span><span class="sxs-lookup"><span data-stu-id="be4ed-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="be4ed-104">Файлы, которые были бы заблокированы правилом, могут запускаться, при этом не ведется запись отчетов или событий.</span><span class="sxs-lookup"><span data-stu-id="be4ed-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="be4ed-105">Исключение применяется ко всем правилам, допускающим эти исключения.</span><span class="sxs-lookup"><span data-stu-id="be4ed-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="be4ed-106">Исключения для сокращения направлений атак (СНА) используют тот же синтаксис, что и исключения антивирусной программы в Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="be4ed-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="be4ed-107">Подробные сведения см. в разделе [Настройки и утверждение исключений для проверки антивирусной программой в Microsoft Defender](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="be4ed-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="be4ed-108">Во избежание проблем просмотрите [распространенные ошибки, которые следует избегать при определении исключений](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="be4ed-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="be4ed-109">Исключения применяются не для всех правил СНА.</span><span class="sxs-lookup"><span data-stu-id="be4ed-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="be4ed-110">Чтобы проверить, поддерживает ли правило исключения, см. таблицу [Правила сокращения направлений атак](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="be4ed-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="be4ed-111">Правила сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="be4ed-111">Attack surface reduction rules</span></span>

<span data-ttu-id="be4ed-112">Все зоны, которые могут быть атакованы злоумышленниками для взлома устройств или сетей организации относятся к направлениям атак.</span><span class="sxs-lookup"><span data-stu-id="be4ed-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="be4ed-113">Сокращение направлений атак усиливает защиту устройств и сетей организации, давая злоумышленникам меньше шансов на совершение атак.</span><span class="sxs-lookup"><span data-stu-id="be4ed-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="be4ed-114">С этим может помочь настройка правил сокращения направлений атак в Microsoft Defender для конечной точки.</span><span class="sxs-lookup"><span data-stu-id="be4ed-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="be4ed-115">Дополнительные сведения см. в статьях:</span><span class="sxs-lookup"><span data-stu-id="be4ed-115">For more information, see:</span></span>

- [<span data-ttu-id="be4ed-116">Сопоставление правила СНА GUID с именем</span><span class="sxs-lookup"><span data-stu-id="be4ed-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="be4ed-117">Требования к правилам СНА:</span><span class="sxs-lookup"><span data-stu-id="be4ed-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="be4ed-118">Windows 10 Pro версии 1709 или более поздней</span><span class="sxs-lookup"><span data-stu-id="be4ed-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="be4ed-119">Windows 10 Корпоративная версии 1709 или более поздней</span><span class="sxs-lookup"><span data-stu-id="be4ed-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="be4ed-120">Windows Server версии 1803 (Semi-Annual Channel) или более поздней</span><span class="sxs-lookup"><span data-stu-id="be4ed-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="be4ed-121">Определение правильного исключения для применения</span><span class="sxs-lookup"><span data-stu-id="be4ed-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="be4ed-122">Найдите eventID 1121 или 1122 в журнале Microsoft-Windows-Windows Defender/Operational.</span><span class="sxs-lookup"><span data-stu-id="be4ed-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="be4ed-123">Вычислите сценарий блокировки и ее контекст, а затем и подтвердите разблокировку сценария.</span><span class="sxs-lookup"><span data-stu-id="be4ed-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="be4ed-124">Считайте значение Path в сведениях о событии, определяющем исключение.</span><span class="sxs-lookup"><span data-stu-id="be4ed-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="be4ed-125">Настройте исключение максимально строго.</span><span class="sxs-lookup"><span data-stu-id="be4ed-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="be4ed-126">При необходимости примените подстановочный символ (например, замените переменную User).</span><span class="sxs-lookup"><span data-stu-id="be4ed-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="be4ed-127">Примените исключение согласно потребностям развертывания.</span><span class="sxs-lookup"><span data-stu-id="be4ed-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="be4ed-128">Подробные сведения см. в разделе [Настройка правил сокращения направлений атак](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="be4ed-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="be4ed-129">Исключение не соблюдается</span><span class="sxs-lookup"><span data-stu-id="be4ed-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="be4ed-130">Определите, допускаются ли исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="be4ed-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="be4ed-131">Подробные сведения см. в разделе [Правила сокращения направлений атак](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="be4ed-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="be4ed-132">Просмотрите примененные исключения и выполните проверку опечаток или неправильно интерпретированных подстановочных символов при помощи данных события.</span><span class="sxs-lookup"><span data-stu-id="be4ed-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="be4ed-133">Дополнительные сведения см. в разделе[Поддерживаемые типы исключений](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="be4ed-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="be4ed-134">если влияние правила слишком большое, попробуйте переместить правило (назад) в режим аудита для дальнейшей проверки.</span><span class="sxs-lookup"><span data-stu-id="be4ed-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="be4ed-135">Подробные сведения см. в разделе [Работа функций Microsoft Defender для конечной точки в режиме аудита](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="be4ed-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="be4ed-136">Чтобы принять обращение в службу поддержки, соберите необходимые данные и примените следующую команду:</span><span class="sxs-lookup"><span data-stu-id="be4ed-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="be4ed-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="be4ed-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="be4ed-138">Дополнительные сведения см. в разделе [Проблемы с подключением компьютеров в Microsoft Defender для конечных точек](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="be4ed-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
