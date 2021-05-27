---
title: Индикаторы не работают в браузере Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651511"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="c9ee7-102">Индикаторы не работают в браузере Edge</span><span class="sxs-lookup"><span data-stu-id="c9ee7-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="c9ee7-103">После создания индикатора он не будет поддерживаться в браузере Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="c9ee7-104">Дополнительные сведения см. в разделе [Создание индикаторов для IP, URL-адресов и доменов](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="c9ee7-105">Шаг 1. Убедитесь в следующем:</span><span class="sxs-lookup"><span data-stu-id="c9ee7-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="c9ee7-106">подтвердите правильность индикатора (нет опечаток в IP/URL-адресе, задано правильное действие и правильные группы RBAC).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="c9ee7-107">Учитывая возможную задержку, следует подождать как минимум 2 часа после создания индикатора.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="c9ee7-108">Подтвердите подключение системы к Microsoft Defender для конечной точки.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="c9ee7-109">Проверьте способность систем взаимодействовать с облаком.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="c9ee7-110">Проверьте подключение и доступность Smartscreen, посетив [проверочный сайт](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="c9ee7-111">Шаг 2. Устранение возможной проблемы</span><span class="sxs-lookup"><span data-stu-id="c9ee7-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="c9ee7-112">Убедитесь, что клиентский компьютер соответствует требованиям.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="c9ee7-113">Дополнительные сведения см. в разделе [Создание индикаторов для IP, URL-адресов и доменов](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="c9ee7-114">Убедитесь, что вы работаете с последней версией браузера Edge.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="c9ee7-115">Чтобы узнать какая версия является последней, см. раздел [Как узнать свою версию Microsoft Edge](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="c9ee7-116">Перезапустите браузер Edge.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="c9ee7-117">Перейдите на сайт, для которого настроен индикатор.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="c9ee7-118">Если сайт выглядит не так, как ожидалось, перейдите к шагу 3.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="c9ee7-119">Шаг 3. Сбор данных</span><span class="sxs-lookup"><span data-stu-id="c9ee7-119">Step 3: Collect data</span></span>

- <span data-ttu-id="c9ee7-120">Сбор диагностических данных **MDEClientAnalyzer**.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="c9ee7-121">Инструкции см. в разделе [Проблемы с подключением компьютеров в Microsoft Defender для конечной точки](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="c9ee7-122">Если установка и сбор данных о трассировке Fiddler для вас не затруднительны, см. раздел [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="c9ee7-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="c9ee7-123">Если вам все же необходима помощь, обратитесь в службу поддержки Майкрософт, выбрав значок "Поддержка", расположенный ниже.</span><span class="sxs-lookup"><span data-stu-id="c9ee7-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
