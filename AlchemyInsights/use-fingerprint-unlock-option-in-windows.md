---
title: Использование параметра Unlock для разблокировки отпечатков пальцев в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588328"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="e5a2c-102">Использование параметра Unlock для разблокировки отпечатков пальцев в Windows 10</span><span class="sxs-lookup"><span data-stu-id="e5a2c-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="e5a2c-103">**Включение отпечатка пальца Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="e5a2c-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="e5a2c-104">Чтобы разблокировать Windows 10 с помощью отпечатка пальца, необходимо настроить отпечаток Windows Hello, добавив (разрешив распознаванию Windows) по крайней мере один палец.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="e5a2c-105">Перейдите в раздел **параметры > учетных записей > параметры входа** (или щелкните [здесь](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="e5a2c-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e5a2c-106">Будут отображены доступные параметры входа.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="e5a2c-107">Например:</span><span class="sxs-lookup"><span data-stu-id="e5a2c-107">For example:</span></span>

    ![Параметры входа.](media/sign-in-options.png)

2. <span data-ttu-id="e5a2c-109">Щелкните значок " **отпечаток Windows Hello**", а затем нажмите кнопку **настроить**.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="e5a2c-110">В окне установки Windows Hello нажмите кнопку **начать работу**.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="e5a2c-111">Будет активирован датчик отпечатков пальцев, и вам будет предложено установить палец на датчик:</span><span class="sxs-lookup"><span data-stu-id="e5a2c-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Датчик отпечатков пальцев.](media/fingerprint-sensor.png)

3. <span data-ttu-id="e5a2c-113">Следуйте инструкциям, чтобы запросить многократное сканирование пальца.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="e5a2c-114">После этого вы сможете добавить других пальцев, которые вы можете использовать для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="e5a2c-115">В следующий раз, когда вы входите в систему Windows 10, вы сможете использовать отпечаток пальца.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="e5a2c-116">**Отпечаток Windows Hello недоступен в качестве варианта входа**</span><span class="sxs-lookup"><span data-stu-id="e5a2c-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="e5a2c-117">Если в параметрах **входа**не отображается отпечаток Windows Hello, это означает, что Windows не знает о каком-либо сканере или сканере отпечатков пальцев, подключенном к компьютеру, или что системная политика запрещает ее использование (например, если ваш компьютер управляется на вашем рабочем месте).</span><span class="sxs-lookup"><span data-stu-id="e5a2c-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="e5a2c-118">Устранение неполадок:</span><span class="sxs-lookup"><span data-stu-id="e5a2c-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="e5a2c-119">Нажмите кнопку " **Пуск** " на панели задач и найдите элемент **Диспетчер устройств**.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="e5a2c-120">Щелкните или нажмите, чтобы открыть **Диспетчер устройств**.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="e5a2c-121">В диспетчере устройств разверните узел биометрические устройства, щелкнув его Шеврон.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Биометрические устройства.](media/biometric-devices.png)

4. <span data-ttu-id="e5a2c-123">Сканер отпечатков пальцев должен быть указан в качестве биометрического устройства, например сканера Синаптикс ВБДИ:</span><span class="sxs-lookup"><span data-stu-id="e5a2c-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Биометрические устройства.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="e5a2c-125">Если сканер отпечатков пальцев не отображается, а сканер интегрирован в компьютер, перейдите на веб-сайт изготовителя компьютера.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="e5a2c-126">В разделе Техническая поддержка для вашей модели компьютера выполните поиск драйвера Windows 10 для сканера, который вы можете установить.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="e5a2c-127">Если сканер отделен от компьютера (подключен через USB), перейдите на веб-сайт изготовителя сканера, чтобы найти и установить программное обеспечение драйвера устройства Windows 10 для модели сканера.</span><span class="sxs-lookup"><span data-stu-id="e5a2c-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
