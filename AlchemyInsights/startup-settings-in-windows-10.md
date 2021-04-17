---
title: Параметры запуска в Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828165"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="ffb88-102">Параметры запуска в Windows 10</span><span class="sxs-lookup"><span data-stu-id="ffb88-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="ffb88-103">**Изменение автоматического запуска приложений при запуске**</span><span class="sxs-lookup"><span data-stu-id="ffb88-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="ffb88-104">Перейдите [в параметры > приложения > запуска](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="ffb88-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="ffb88-105">Убедитесь, что любое приложение, которое необходимо запустить при запуске, **включено.**</span><span class="sxs-lookup"><span data-stu-id="ffb88-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="ffb88-106">**Добавление приложения для автоматического запуска при запуске**</span><span class="sxs-lookup"><span data-stu-id="ffb88-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="ffb88-107">Нажмите кнопку **Пуск** или нажмите кнопку Пуск и найдите приложение, которое необходимо запустить при запуске.</span><span class="sxs-lookup"><span data-stu-id="ffb88-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="ffb88-108">Щелкните правой кнопкой мыши приложение, нажмите **кнопку Больше,** а затем нажмите **кнопку Открыть расположение файла**.</span><span class="sxs-lookup"><span data-stu-id="ffb88-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="ffb88-109">Это открывает расположение, в котором сохранен ярлык приложения.</span><span class="sxs-lookup"><span data-stu-id="ffb88-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="ffb88-110">Если нет возможности для расположения открытого файла, это означает, что приложение не может работать при запуске.</span><span class="sxs-lookup"><span data-stu-id="ffb88-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="ffb88-111">С открытым расположением файла нажмите **клавишу логотипа Windows + R,** введите оболочку:запуск, а затем нажмите **кнопку ОК**. </span><span class="sxs-lookup"><span data-stu-id="ffb88-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="ffb88-112">Это открывает папку Startup.</span><span class="sxs-lookup"><span data-stu-id="ffb88-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="ffb88-113">Скопируйте и вложите ярлык в приложение из расположения файла в папку Startup.</span><span class="sxs-lookup"><span data-stu-id="ffb88-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="ffb88-114">**Расширенные параметры запуска (включая безопасный режим, параметры UEFI и загрузку с другого устройства)**</span><span class="sxs-lookup"><span data-stu-id="ffb88-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="ffb88-115">Сохраните работу и закройте все открытые документы, так как эти действия перезапустят компьютер.</span><span class="sxs-lookup"><span data-stu-id="ffb88-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="ffb88-116">Перейдите [в параметры > обновления & безопасности > восстановления](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="ffb88-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="ffb88-117">В **advanced startup** нажмите **кнопку Перезапустить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="ffb88-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="ffb88-118">После перезапуска компьютера на экран параметра Выберите:</span><span class="sxs-lookup"><span data-stu-id="ffb88-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="ffb88-119">Чтобы загрузиться с устройства, например USB-накопителя, нажмите **кнопку Используйте устройство.**</span><span class="sxs-lookup"><span data-stu-id="ffb88-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="ffb88-120">Чтобы ввести параметры UEFI (иногда называемую установкой BIOS), нажмите кнопку Устранение неполадок > расширенные параметры > **UEFI.**</span><span class="sxs-lookup"><span data-stu-id="ffb88-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="ffb88-121">Чтобы ввести **безопасный** режим или изменить расширенные параметры запуска, нажмите кнопку Устранение неполадок > расширенные параметры > параметров запуска, а затем нажмите кнопку **Перезапустить**.</span><span class="sxs-lookup"><span data-stu-id="ffb88-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="ffb88-122">Возможно, вам будет предложено ввести ключ [восстановления BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="ffb88-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="ffb88-123">После повторного перезапуска компьютера щелкните параметр запуска, который вы хотите использовать.</span><span class="sxs-lookup"><span data-stu-id="ffb88-123">After your PC restarts again, click the startup setting you want to use.</span></span>