---
title: Освобождение места на диске в Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505369"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="b04eb-102">Освобождение места на диске в Windows 10</span><span class="sxs-lookup"><span data-stu-id="b04eb-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="b04eb-103">Вот два способа освободить место на диске в Windows:</span><span class="sxs-lookup"><span data-stu-id="b04eb-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="b04eb-104">Освобождение места на диске в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b04eb-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="b04eb-105">Освободите место для обновлений Windows 10 с помощью внешнего запоминающего устройства.</span><span class="sxs-lookup"><span data-stu-id="b04eb-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="b04eb-106">Если после очистки диска по-прежнему остается мало места на диске, возможно, папка Temp быстро заполняется файлами приложений (APPX), используемыми Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="b04eb-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="b04eb-107">Чтобы устранить эту проблему, сбросьте Store, очистите кэш Store и запустите средство устранения неполадок Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="b04eb-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="b04eb-108">Прежде чем приступить к этим шагам, убедитесь, что Microsoft Store закрыт.</span><span class="sxs-lookup"><span data-stu-id="b04eb-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="b04eb-109">**Шаг 1. Сброс Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="b04eb-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="b04eb-110">**Примечание.** На устройстве безвозвратно удаляются данные приложения, включая настройки и данные для входа.</span><span class="sxs-lookup"><span data-stu-id="b04eb-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="b04eb-111">Выберите **Пуск** > **Параметры** > **Приложения** > **Приложения и функции**.</span><span class="sxs-lookup"><span data-stu-id="b04eb-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="b04eb-112">В списке приложений найдите и выберите Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="b04eb-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="b04eb-113">Выберите элемент **Дополнительные параметры**.</span><span class="sxs-lookup"><span data-stu-id="b04eb-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="b04eb-114">Прокрутите вниз и выберите **Сбросить**, а затем **Подтвердить сброс**.</span><span class="sxs-lookup"><span data-stu-id="b04eb-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="b04eb-115">**Шаг 2. Очистка кэша Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="b04eb-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="b04eb-116">Нажмите клавишу с логотипом Windows + R, чтобы открыть диалоговое окно "Выполнить".</span><span class="sxs-lookup"><span data-stu-id="b04eb-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="b04eb-117">Введите wsreset.exe и нажмите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b04eb-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="b04eb-118">Откроется пустое окно командной строки.</span><span class="sxs-lookup"><span data-stu-id="b04eb-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="b04eb-119">Примерно через 10 секунд окно закроется, а Store откроется автоматически.</span><span class="sxs-lookup"><span data-stu-id="b04eb-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="b04eb-120">**Шаг 3. Сброс Центра обновления Windows**</span><span class="sxs-lookup"><span data-stu-id="b04eb-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="b04eb-121">Выберите **Пуск** > **Параметры** > **Обновление и безопасность** > **Устранение неполадок**.</span><span class="sxs-lookup"><span data-stu-id="b04eb-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="b04eb-122">Прокрутите страницу вниз и выберите **Центр обновления Windows** в списке и выберите **Запустить средство устранения неполадок**.</span><span class="sxs-lookup"><span data-stu-id="b04eb-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="b04eb-123">Перезагрузите компьютер и проверьте, сохраняется ли проблема.</span><span class="sxs-lookup"><span data-stu-id="b04eb-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

