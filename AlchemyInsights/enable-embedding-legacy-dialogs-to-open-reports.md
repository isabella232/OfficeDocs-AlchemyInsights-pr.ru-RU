---
title: Разрешение внедрения устаревших диалоговых окон для открытия отчетов
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814277"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="2c901-102">Разрешение внедрения устаревших диалоговых окон для открытия отчетов</span><span class="sxs-lookup"><span data-stu-id="2c901-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="2c901-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="2c901-103">**Symptom**</span></span>

<span data-ttu-id="2c901-104">Пользователям не удается открыть отчеты.</span><span class="sxs-lookup"><span data-stu-id="2c901-104">Users are unable to open reports.</span></span> <span data-ttu-id="2c901-105">"Возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="2c901-105">"Something has gone wrong.</span></span> <span data-ttu-id="2c901-106">Подробности см. в технических сведениях".</span><span class="sxs-lookup"><span data-stu-id="2c901-106">Check technical details for more details."</span></span>

<span data-ttu-id="2c901-107">**Причина**</span><span class="sxs-lookup"><span data-stu-id="2c901-107">**Cause**</span></span>

<span data-ttu-id="2c901-108">Отчеты не загружаются в UCI с ошибкой "Дескриптор формы имеет значение null или не определен".</span><span class="sxs-lookup"><span data-stu-id="2c901-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="2c901-109">Отчетам в UCI по-прежнему требуются устаревшие диалоговые окна, поэтому в системе пользователя должен быть включен параметр *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="2c901-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="2c901-110">**Решение**</span><span class="sxs-lookup"><span data-stu-id="2c901-110">**Solution**</span></span>

1. <span data-ttu-id="2c901-111">Выберите **Параметры >Администрирование > Параметры системы > вкладка "Общее"**.</span><span class="sxs-lookup"><span data-stu-id="2c901-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="2c901-112">Присвойте параметру "Разрешить внедрение некоторых устаревших диалогов в браузерный клиент с единым интерфейсом" значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="2c901-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
