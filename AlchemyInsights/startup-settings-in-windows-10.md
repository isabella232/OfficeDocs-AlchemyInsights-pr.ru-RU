---
title: Параметры запуска в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409232"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="fead3-102">Параметры запуска в Windows 10</span><span class="sxs-lookup"><span data-stu-id="fead3-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="fead3-103">**Изменение приложений, запускаемых автоматически при запуске**</span><span class="sxs-lookup"><span data-stu-id="fead3-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="fead3-104">Перейдите в раздел [параметры > приложения > запуска](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="fead3-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="fead3-105">Убедитесь, что приложение, которое вы хотите запускать при запуске, **включено.**</span><span class="sxs-lookup"><span data-stu-id="fead3-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="fead3-106">**Добавление приложения для автоматического запуска при запуске**</span><span class="sxs-lookup"><span data-stu-id="fead3-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="fead3-107">Нажмите кнопку **Пуск** и найдите приложение, которое необходимо запустить при запуске.</span><span class="sxs-lookup"><span data-stu-id="fead3-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="fead3-108">Щелкните приложение правой кнопкой мыши, выберите пункт **Дополнительно**и щелкните **открыть расположение файла**.</span><span class="sxs-lookup"><span data-stu-id="fead3-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="fead3-109">Откроется расположение, в котором сохраняется ярлык для приложения.</span><span class="sxs-lookup"><span data-stu-id="fead3-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="fead3-110">Если параметр открыть расположение файлов отсутствует, это означает, что приложение не запускается при запуске.</span><span class="sxs-lookup"><span data-stu-id="fead3-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="fead3-111">Откройте расположение файла, нажмите клавишу с **логотипом Windows + R**, введите **Shell: Startup**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fead3-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="fead3-112">Откроется папка "Автозагрузка".</span><span class="sxs-lookup"><span data-stu-id="fead3-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="fead3-113">Скопируйте и вставьте ярлык в приложение из расположения файла в папку "Автозагрузка".</span><span class="sxs-lookup"><span data-stu-id="fead3-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="fead3-114">**Расширенные варианты запуска (включая безопасный режим, параметры UEFI и загрузку с другого устройства)**</span><span class="sxs-lookup"><span data-stu-id="fead3-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="fead3-115">Сохраните работу и закройте все открытые документы, так как эти действия приведут к перезапуску компьютера.</span><span class="sxs-lookup"><span data-stu-id="fead3-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="fead3-116">Перейдите в раздел [параметры > обновление & безопасность > восстановление](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="fead3-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="fead3-117">В разделе **Дополнительная загрузка**нажмите кнопку **Перезапустить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="fead3-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="fead3-118">После перезагрузки компьютера на экран Выбор параметров:</span><span class="sxs-lookup"><span data-stu-id="fead3-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="fead3-119">Для загрузки с устройства, такого как USB-накопитель, щелкните **использовать устройство**.</span><span class="sxs-lookup"><span data-stu-id="fead3-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="fead3-120">Чтобы ввести параметры UEFI (иногда называемые программой установки BIOS), нажмите кнопку **Устранение неполадок > дополнительные параметры > параметры встроенного по UEFI**.</span><span class="sxs-lookup"><span data-stu-id="fead3-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="fead3-121">Чтобы войти в безопасный режим или изменить дополнительные параметры запуска, щелкните ссылку **Устранение неполадок > дополнительные параметры > параметры запуска**, а затем нажмите кнопку **перезапустить**.</span><span class="sxs-lookup"><span data-stu-id="fead3-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="fead3-122">Вам может быть предложено ввести [ключ восстановления BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="fead3-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="fead3-123">После повторного перезапуска компьютера выберите параметр запуска, который необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="fead3-123">After your PC restarts again, click the startup setting you want to use.</span></span>