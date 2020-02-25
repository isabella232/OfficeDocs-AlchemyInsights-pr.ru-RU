---
title: Устранение неполадок Bluetooth в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268706"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="0fb6a-102">Устранение неполадок Bluetooth в Windows 10</span><span class="sxs-lookup"><span data-stu-id="0fb6a-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="0fb6a-103">Если значок Bluetooth отсутствует или не удается включить или отключить Bluetooth, возможно, вы захотите запустить средство устранения неполадок Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="0fb6a-104">[Откройте параметры устранения неполадок](ms-settings:troubleshoot), выберите **Bluetooth** в разделе **Поиск и устранение других проблем**нажмите **запустить средство устранения неполадок**.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="0fb6a-105">Если значок Bluetooth не отображается, но Bluetooth отображается в диспетчере устройств:</span><span class="sxs-lookup"><span data-stu-id="0fb6a-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="0fb6a-106">В диспетчере устройств щелкните **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="0fb6a-107">Нажмите и удерживайте (или щелкните правой кнопкой мыши) имя адаптера Bluetooth и выберите команду **удалить устройство**.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="0fb6a-108">Завершите работу устройства с Windows, подождите несколько секунд, а затем снова включите его.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="0fb6a-109">Windows попытается переустановить драйвер.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="0fb6a-110">Если вы недавно установили обновления Windows 10 или обновили до Windows 10, вы можете проверить наличие обновлений драйверов:</span><span class="sxs-lookup"><span data-stu-id="0fb6a-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="0fb6a-111">В диспетчере устройств щелкните **Bluetooth**, а затем щелкните имя адаптера Bluetooth (которое может содержать слово "Radio").</span><span class="sxs-lookup"><span data-stu-id="0fb6a-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="0fb6a-112">Нажмите и удерживайте (или щелкните правой кнопкой мыши) адаптер Bluetooth, а затем щелкните **Обновить поиск драйверов** > **автоматически для обновленного программного обеспечения драйвера**.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="0fb6a-113">Выполните действия, а затем нажмите кнопку **Закрыть**.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="0fb6a-114">Если Windows не удается найти новый драйвер Bluetooth, посетите веб-сайт производителя компьютера и скачайте последнюю версию драйвера Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="0fb6a-115">После того как вы Скачайте его, нажмите кнопку **Обновить драйвер** > . > **Обзор программного обеспечения для драйвера\*\*\*\*найдите** расположение, в котором хранятся файлы драйверов > **ОК** > **, а затем следуйте**инструкциям по установке.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="0fb6a-116">После установки обновленного драйвера перезапустите компьютер и проверьте, устранена ли проблема с подключением.</span><span class="sxs-lookup"><span data-stu-id="0fb6a-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="0fb6a-117">Более подробную информацию об устранении неполадок Bluetooth можно найти в полной статье [Устранение неполадок Bluetooth в Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="0fb6a-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
