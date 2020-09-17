---
title: Разрешение внедрения устаревших диалоговых окон для открытия отчетов
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806448"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="b7a23-102">Разрешение внедрения устаревших диалоговых окон для открытия отчетов</span><span class="sxs-lookup"><span data-stu-id="b7a23-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="b7a23-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="b7a23-103">**Symptom**</span></span>

<span data-ttu-id="b7a23-104">Пользователям не удается открыть отчеты.</span><span class="sxs-lookup"><span data-stu-id="b7a23-104">Users are unable to open reports.</span></span> <span data-ttu-id="b7a23-105">"Возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="b7a23-105">"Something has gone wrong.</span></span> <span data-ttu-id="b7a23-106">Подробности см. в технических сведениях".</span><span class="sxs-lookup"><span data-stu-id="b7a23-106">Check technical details for more details."</span></span>

<span data-ttu-id="b7a23-107">**Причина**</span><span class="sxs-lookup"><span data-stu-id="b7a23-107">**Cause**</span></span>

<span data-ttu-id="b7a23-108">Отчеты не загружаются в UCI с ошибкой "Дескриптор формы имеет значение null или не определен".</span><span class="sxs-lookup"><span data-stu-id="b7a23-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="b7a23-109">Отчетам в UCI по-прежнему требуются устаревшие диалоговые окна, поэтому в системе пользователя должен быть включен параметр *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="b7a23-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="b7a23-110">**Решение**</span><span class="sxs-lookup"><span data-stu-id="b7a23-110">**Solution**</span></span>

1. <span data-ttu-id="b7a23-111">Выберите **Параметры >Администрирование > Параметры системы > вкладка "Общее"**.</span><span class="sxs-lookup"><span data-stu-id="b7a23-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="b7a23-112">Присвойте параметру "Разрешить внедрение некоторых устаревших диалогов в браузерный клиент с единым интерфейсом" значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="b7a23-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
