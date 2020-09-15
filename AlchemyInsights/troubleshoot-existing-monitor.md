---
title: Устранение неполадок существующего монитора
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690724"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="2ecf4-102">Устранение неполадок существующего монитора</span><span class="sxs-lookup"><span data-stu-id="2ecf4-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="2ecf4-103">Воспользуйтесь этими решениями, чтобы устранить неполадки с монитором.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="2ecf4-104">**Обновите экран монитора:**</span><span class="sxs-lookup"><span data-stu-id="2ecf4-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="2ecf4-105">Одновременно используйте следующие клавиши: клавиша Windows + Ctrl + Shift + B. При этом будет обновлена связь с драйвером графической подсистемы.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="2ecf4-106">Мониторы мигают на мгновениях и будут возвращаться через несколько секунд.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="2ecf4-107">**Устранение неполадок оборудования монитора:**</span><span class="sxs-lookup"><span data-stu-id="2ecf4-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="2ecf4-108">Отсоедините кабель, соединяющий компьютер с монитором, и снова подключите его.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="2ecf4-109">Отключите все несущественные устройства от компьютера (например, адаптеры или стыковочные устройства).</span><span class="sxs-lookup"><span data-stu-id="2ecf4-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="2ecf4-110">**Если вы недавно установили обновление на компьютере, вы можете откатить свой драйвер экрана:**</span><span class="sxs-lookup"><span data-stu-id="2ecf4-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="2ecf4-111">Нажмите кнопку **Пуск**, введите **Диспетчер устройств**и выберите **Диспетчер устройств** из результатов.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="2ecf4-112">Разверните раздел **Видеоадаптеры** , щелкните правой кнопкой мыши видеоадаптер, смешивать и выберите **свойства**.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="2ecf4-113">Перейдите на вкладку **Driver (драйвер** ) и выберите пункт **вернуть драйвер**.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="2ecf4-114">Примечание. Если этот параметр недоступен или неактивен, выберите пункт **нет** в списке ниже, чтобы перейти к следующему шагу.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="2ecf4-115">Для вступления изменений в силу может потребоваться перезагрузка компьютера.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="2ecf4-116">**Удалите и переустановите драйвер экрана.**</span><span class="sxs-lookup"><span data-stu-id="2ecf4-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="2ecf4-117">Нажмите кнопку **Пуск**, введите **Диспетчер устройств**и выберите **Диспетчер устройств** из результатов.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="2ecf4-118">Разверните раздел **Видеоадаптеры** , щелкните правой кнопкой мыши видеоадаптер смешивать и выберите пункт **удалить устройство**.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="2ecf4-119">Установите флажок рядом с пунктом **удалить драйвер для этого устройства** и нажмите кнопку **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="2ecf4-120">Примечание. вам может быть предложено перезапустить компьютер на этом этапе.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="2ecf4-121">Перед перезагрузкой обязательно запишите остальные инструкции.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="2ecf4-122">Снова откройте Диспетчер устройств.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="2ecf4-123">Разверните раздел **адаптеры отображения** , щелкните правой кнопкой мыши видеоадаптер и выберите команду **Обновить драйвер**.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="2ecf4-124">Выберите **автоматически Поиск по драйверу обновления** и следуйте инструкциям по установке.</span><span class="sxs-lookup"><span data-stu-id="2ecf4-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>