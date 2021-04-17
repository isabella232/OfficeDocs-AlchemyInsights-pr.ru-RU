---
title: Устранение проблем со звуком в Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833304"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="71b2c-102">Устранение неполадок со звуком в Windows 10</span><span class="sxs-lookup"><span data-stu-id="71b2c-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="71b2c-103">**Запуск звукового устранения неполадок**</span><span class="sxs-lookup"><span data-stu-id="71b2c-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="71b2c-104">Откройте [параметры устранения неполадок.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="71b2c-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="71b2c-105">Выберите **Воспроизведение звука**  >  **Запустите устранение неполадок.**</span><span class="sxs-lookup"><span data-stu-id="71b2c-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="71b2c-106">**Настройка устройства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="71b2c-106">**Set the default device**</span></span>

<span data-ttu-id="71b2c-107">При подключении к аудио-устройству с помощью USB или HDMI может потребоваться установить это устройство по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="71b2c-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="71b2c-108">Откройте   >  **начните звук,** а затем выберите **звук** или **изменение** системных звуков из списка результатов.</span><span class="sxs-lookup"><span data-stu-id="71b2c-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="71b2c-109">На **вкладке Воспроизведение** выберите устройство, выберите **набор** по умолчанию и выберите **ОК.**</span><span class="sxs-lookup"><span data-stu-id="71b2c-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="71b2c-110">**Проверка кабелей, громкости, динамиков и наушников**</span><span class="sxs-lookup"><span data-stu-id="71b2c-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="71b2c-111">Проверьте подключение динамика и наушников к свободным кабелям и убедитесь, что они подключены к правильному разъему.</span><span class="sxs-lookup"><span data-stu-id="71b2c-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="71b2c-112">Проверьте уровень мощности и громкости и попробуйте включите все элементы управления громкости.</span><span class="sxs-lookup"><span data-stu-id="71b2c-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="71b2c-113">Некоторые динамики и приложения имеют собственные элементы управления громкости; возможно, вам придется проверить их все, чтобы убедиться, что они на правильных уровнях.</span><span class="sxs-lookup"><span data-stu-id="71b2c-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="71b2c-114">Попробуйте подключиться с помощью другого USB-порта.</span><span class="sxs-lookup"><span data-stu-id="71b2c-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="71b2c-115">**Примечание.** Помните, что динамики могут не работать при подключении наушников.</span><span class="sxs-lookup"><span data-stu-id="71b2c-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="71b2c-116">**Проверка диспетчера устройств**</span><span class="sxs-lookup"><span data-stu-id="71b2c-116">**Check Device Manager**</span></span>

<span data-ttu-id="71b2c-117">Чтобы убедиться, что драйверы устарели:</span><span class="sxs-lookup"><span data-stu-id="71b2c-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="71b2c-118">Выберите **Начните,** введите **диспетчер устройств,** а затем выберите **диспетчер** устройств из списка результатов.</span><span class="sxs-lookup"><span data-stu-id="71b2c-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="71b2c-119">В **контроллерах звука, видео** и игр выберите звуковую карточку, откройте ее, выберите вкладку **Driver** и выберите **Драйвер обновления**.</span><span class="sxs-lookup"><span data-stu-id="71b2c-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="71b2c-120">**Примечание.** Если Windows не находит новый драйвер, найдите его на веб-сайте производителя устройств и следуйте их инструкциям.</span><span class="sxs-lookup"><span data-stu-id="71b2c-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="71b2c-121">**Переустановка драйвера**</span><span class="sxs-lookup"><span data-stu-id="71b2c-121">**Reinstall the driver**</span></span>

<span data-ttu-id="71b2c-122">Если вы не можете обновить с помощью диспетчера устройств или найти новый драйвер на веб-сайте производителя, попробуйте следующие действия:</span><span class="sxs-lookup"><span data-stu-id="71b2c-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="71b2c-123">В диспетчере устройств щелкните правой кнопкой мыши (или нажмите кнопку и удерживайте) драйвер звука и выберите **Uninstall**.</span><span class="sxs-lookup"><span data-stu-id="71b2c-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="71b2c-124">Перезапустите устройство, и Windows попытается переустановить драйвер.</span><span class="sxs-lookup"><span data-stu-id="71b2c-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="71b2c-125">Если переустановка драйвера не работает, попробуйте использовать общий драйвер звука, который поставляется с Windows.</span><span class="sxs-lookup"><span data-stu-id="71b2c-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="71b2c-126">В диспетчере устройств щелкните правой кнопкой мыши (или нажмите кнопку и удерживайте) драйвер звука > Обновление программного обеспечения драйвера Просмотр компьютера для программного обеспечения драйвера Позвольте мне выбрать из списка драйверов устройств на моем компьютере, выберите аудио устройство высокой четкости, выберите Далее , и следуйте инструкциям по его  >    >  установке.  </span><span class="sxs-lookup"><span data-stu-id="71b2c-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
