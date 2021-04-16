---
title: Использование параметра разблокировки отпечатков пальцев в Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796690"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="51655-102">Использование параметра разблокировки отпечатков пальцев в Windows 10</span><span class="sxs-lookup"><span data-stu-id="51655-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="51655-103">**Включить отпечаток Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="51655-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="51655-104">Чтобы разблокировать Windows 10 с помощью отпечатка пальца, необходимо настроить windows Hello Fingerprint, добавив (позволяя Windows научиться распознавать) по крайней мере один палец.</span><span class="sxs-lookup"><span data-stu-id="51655-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="51655-105">Перейдите **к параметрам > учетных записей > параметров** регистрации (или нажмите [здесь).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="51655-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="51655-106">Будут перечислены доступные параметры входов.</span><span class="sxs-lookup"><span data-stu-id="51655-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="51655-107">Например,</span><span class="sxs-lookup"><span data-stu-id="51655-107">For example:</span></span>

    ![Параметры входов.](media/sign-in-options.png)

2. <span data-ttu-id="51655-109">Щелкните или нажмите **кнопку Windows Hello Fingerprint**, а затем нажмите **кнопку Настройка**.</span><span class="sxs-lookup"><span data-stu-id="51655-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="51655-110">В окне установки Windows Hello нажмите кнопку **Начало** работы.</span><span class="sxs-lookup"><span data-stu-id="51655-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="51655-111">Датчик отпечатков пальцев активируется, и вам будет предложено разместить палец на датчике:</span><span class="sxs-lookup"><span data-stu-id="51655-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Датчик отпечатков пальцев.](media/fingerprint-sensor.png)

3. <span data-ttu-id="51655-113">Следуйте инструкциям, которые будут просить вас повторно сканировать палец.</span><span class="sxs-lookup"><span data-stu-id="51655-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="51655-114">После этого у вас будет возможность добавить другие пальцы, которые можно использовать для регистрации.</span><span class="sxs-lookup"><span data-stu-id="51655-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="51655-115">При следующем входе в Windows 10 у вас будет возможность использовать для этого свой отпечаток пальца.</span><span class="sxs-lookup"><span data-stu-id="51655-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="51655-116">**Windows Hello Fingerprint недоступна в качестве параметра входной**</span><span class="sxs-lookup"><span data-stu-id="51655-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="51655-117">Если windows Hello Fingerprint не отображается в качестве параметра в параметрах **Вход,** это означает, что Windows не знает о считывателье или сканере отпечатков пальцев, подключенных к компьютеру, или о том, что системная политика не позволяет использовать его (если, например, компьютер управляется на рабочем месте).</span><span class="sxs-lookup"><span data-stu-id="51655-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="51655-118">Устранение неполадок:</span><span class="sxs-lookup"><span data-stu-id="51655-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="51655-119">Выберите **кнопку Начните** в панели задач и выберите **диспетчер устройств.**</span><span class="sxs-lookup"><span data-stu-id="51655-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="51655-120">Щелкните или нажмите кнопку, чтобы **открыть диспетчер устройств.**</span><span class="sxs-lookup"><span data-stu-id="51655-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="51655-121">В диспетчере устройств разойдитесь по биометрическим устройствам, щелкнув его шеврон.</span><span class="sxs-lookup"><span data-stu-id="51655-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Биометрические устройства.](media/biometric-devices.png)

4. <span data-ttu-id="51655-123">Сканер отпечатков пальцев должен быть указан как биометрическое устройство, например сканер WBDI Synaptics:</span><span class="sxs-lookup"><span data-stu-id="51655-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Биометрические устройства.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="51655-125">Если сканер отпечатков пальцев не показан и сканер интегрирован в компьютер, перейдите на веб-сайт производителя ПК.</span><span class="sxs-lookup"><span data-stu-id="51655-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="51655-126">В разделе техническая поддержка для модели ПК ищите драйвер Windows 10 для сканера, который можно установить.</span><span class="sxs-lookup"><span data-stu-id="51655-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="51655-127">Если сканер отделен от компьютера (присоединен через USB), перейдите на веб-сайт производителя сканера, чтобы найти и установить программное обеспечение драйвера устройства Windows 10 для модели сканера.</span><span class="sxs-lookup"><span data-stu-id="51655-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
