---
title: Устранение неполадок со звуком в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750356"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="08c5a-102">Устранение проблем со звуком в Windows 10</span><span class="sxs-lookup"><span data-stu-id="08c5a-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="08c5a-103">**Запуск средства устранения неполадок со звуком**</span><span class="sxs-lookup"><span data-stu-id="08c5a-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="08c5a-104">Откройте [параметры устранения неполадок](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="08c5a-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="08c5a-105">Нажмите кнопку **Воспроизведение звука**  >  **запустите средство устранения неполадок**.</span><span class="sxs-lookup"><span data-stu-id="08c5a-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="08c5a-106">**Задание устройства по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="08c5a-106">**Set the default device**</span></span>

<span data-ttu-id="08c5a-107">Если вы подключаетесь к звуковому устройству с помощью USB или HDMI, вам может потребоваться установить это устройство по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="08c5a-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="08c5a-108">Откройте **меню "Пуск**"  >  **Sound**, выберите **звук** или **изменить звуки системы** из списка результатов.</span><span class="sxs-lookup"><span data-stu-id="08c5a-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="08c5a-109">На вкладке **Воспроизведение** выберите устройство, нажмите **установить по умолчанию**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="08c5a-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="08c5a-110">**Проверка кабелей, громкости, динамиков и наушников**</span><span class="sxs-lookup"><span data-stu-id="08c5a-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="08c5a-111">Проверьте подключения динамиков и наушников для свободных кабелей и убедитесь, что они подключены к правильному разъему.</span><span class="sxs-lookup"><span data-stu-id="08c5a-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="08c5a-112">Проверьте уровни питания и громкости и попытайтесь отключить все регуляторы громкости.</span><span class="sxs-lookup"><span data-stu-id="08c5a-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="08c5a-113">У некоторых динамиков и приложений есть собственные регуляторы громкости; Вам может потребоваться проверить все, чтобы убедиться, что они находятся на правильных уровнях.</span><span class="sxs-lookup"><span data-stu-id="08c5a-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="08c5a-114">Попробуйте подключиться с помощью другого USB-порта.</span><span class="sxs-lookup"><span data-stu-id="08c5a-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="08c5a-115">**Note**: Помните, что динамики могут не работать, если подключены наушники.</span><span class="sxs-lookup"><span data-stu-id="08c5a-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="08c5a-116">**Проверка диспетчера устройств**</span><span class="sxs-lookup"><span data-stu-id="08c5a-116">**Check Device Manager**</span></span>

<span data-ttu-id="08c5a-117">Чтобы убедиться, что драйверы обновлены, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="08c5a-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="08c5a-118">Нажмите кнопку **Пуск**, введите **Диспетчер устройств**, а затем выберите **Диспетчер устройств** из списка результатов.</span><span class="sxs-lookup"><span data-stu-id="08c5a-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="08c5a-119">В разделе **Звуковые, видео и игровые устройства**выберите свою звуковую карту, откройте ее, перейдите на вкладку **драйвер** и выберите **Обновить драйвер**.</span><span class="sxs-lookup"><span data-stu-id="08c5a-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="08c5a-120">**Note**: Если Windows не находит новый драйвер, найдите его на веб-сайте изготовителя устройства и следуйте инструкциям.</span><span class="sxs-lookup"><span data-stu-id="08c5a-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="08c5a-121">**Переустановка драйвера**</span><span class="sxs-lookup"><span data-stu-id="08c5a-121">**Reinstall the driver**</span></span>

<span data-ttu-id="08c5a-122">Если вы не можете обновить с помощью диспетчера устройств или найти новый драйвер на веб-сайте изготовителя, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="08c5a-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="08c5a-123">В диспетчере устройств щелкните правой кнопкой мыши (или нажмите и удерживайте) звуковой драйвер и выберите **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="08c5a-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="08c5a-124">Перезапустите устройство, и Windows предпримет попытку переустановить драйвер.</span><span class="sxs-lookup"><span data-stu-id="08c5a-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="08c5a-125">Если переустановка драйвера не работает, попробуйте использовать универсальный звуковой драйвер, поставляемый с Windows.</span><span class="sxs-lookup"><span data-stu-id="08c5a-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="08c5a-126">В диспетчере устройств щелкните правой кнопкой мыши (или нажмите и удерживайте) аудио-драйвер > **Обновление драйверов. Обзор программного**обеспечения  >  **для драйверов**. Выберите в  >  **списке драйвер устройства**, а **затем нажмите кнопку** **Далее**и следуйте инструкциям по установке.</span><span class="sxs-lookup"><span data-stu-id="08c5a-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
