---
title: Оценка существующей среды браузера и определение целей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530128"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="2bfb8-102">Оценка существующей среды браузера и определение целей</span><span class="sxs-lookup"><span data-stu-id="2bfb8-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="2bfb8-103">Изучите текущее состояние браузера и концепцию проекта, чтобы все заинтересованные лица совместно работали над достижением одной и той же цели.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="2bfb8-104">Выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-104">Follow these steps:</span></span>

1. <span data-ttu-id="2bfb8-105">Определите текущее состояние.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-105">Define your current state.</span></span> <span data-ttu-id="2bfb8-106">Примите во внимание следующее.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-106">Consider the following:</span></span>
- <span data-ttu-id="2bfb8-107">Какие браузеры сейчас развернуты в вашей среде?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="2bfb8-108">Какой браузер установлен в качестве браузера по умолчанию?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="2bfb8-109">Требуется ли использовать Internet Explorer для некоторых приложений?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="2bfb8-110">Используете ли вы сегодня список сайтов в режиме предприятия для настройки Internet Explorer?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="2bfb8-111">Какие платформы ОС (например, Windows 10 или macOS) поддерживаются в вашей среде?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="2bfb8-112">Какие средства управления используются для управления браузерами?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="2bfb8-113">Кто отвечает за настройку браузера и управление им?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="2bfb8-114">Каков процесс проверки совместимости браузеров?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="2bfb8-115">Определите цели развертывания.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-115">Define the goals for your deployment.</span></span> <span data-ttu-id="2bfb8-116">Примите во внимание следующее.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="2bfb8-117">Хотите ли вы [установить Microsoft Edge в качестве браузера по умолчанию](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="2bfb8-118">Хотите ли вы скрыть устаревшую версию Microsoft Edge или [оставить ее доступной для пользователей](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="2bfb8-119">Как вы будете [настраивать Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="2bfb8-120">Какие функции необходимо настроить в рамках первоначального развертывания?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="2bfb8-121">Каков процесс устранения выявленных проблем совместимости или конфигурации?</span><span class="sxs-lookup"><span data-stu-id="2bfb8-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="2bfb8-122">Определите необходимые функции, например:</span><span class="sxs-lookup"><span data-stu-id="2bfb8-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="2bfb8-123">Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="2bfb8-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="2bfb8-124">Режим Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="2bfb8-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="2bfb8-125">Проверка подлинности и синхронизация</span><span class="sxs-lookup"><span data-stu-id="2bfb8-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="2bfb8-126">После выполнения этих действий можно приступать к планированию стратегии развертывания.</span><span class="sxs-lookup"><span data-stu-id="2bfb8-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
