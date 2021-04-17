---
title: Устранение неполадок существующего монитора
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824592"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="cc0e7-102">Устранение неполадок существующего монитора</span><span class="sxs-lookup"><span data-stu-id="cc0e7-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="cc0e7-103">Попробуйте эти решения для устранения неполадок монитора.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="cc0e7-104">**Обновление дисплея монитора:**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="cc0e7-105">Нажмите клавиши: Windows Key + Ctrl + Shift + B. Это позволит обновить связь с драйвером графики.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="cc0e7-106">Мониторы будут мигать и возвращаться через несколько секунд.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="cc0e7-107">**Устранение неполадок монитор оборудования:**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="cc0e7-108">Отсоедините кабель, соединяющий компьютер с монитором, и снова подключите его.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="cc0e7-109">Отсоедините от компьютера все не особо важные устройства (например, адаптеры или док-станции).</span><span class="sxs-lookup"><span data-stu-id="cc0e7-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="cc0e7-110">**Если недавно установлено обновление на компьютере, можно откатить драйвер отображения:**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="cc0e7-111">Выберите **Начните,** введите **диспетчер устройств** и выберите диспетчер **устройств** из результатов.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="cc0e7-112">**Расширите раздел Адаптеры** отображения, щелкните правой кнопкой мыши адаптер отображения и выберите **Свойства.**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="cc0e7-113">Перейдите на **вкладку Драйвер** и выберите **откат драйвера**.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="cc0e7-114">Примечание. Если этот параметр не доступен или не имеет серого цвета, выберите **"Нет"** из параметров ниже, чтобы перейти к следующему шагу.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="cc0e7-115">Возможно, вам потребуется перезапустить компьютер до того, как эти изменения вступает в силу.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="cc0e7-116">**Удалить и переустановить драйвер отображения:**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="cc0e7-117">Выберите **Начните,** введите **диспетчер устройств** и выберите диспетчер **устройств** из результатов.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="cc0e7-118">**Расширите раздел Адаптеры** отображения, щелкните правой кнопкой мыши адаптер отображения и выберите устройство **Uninstall.**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="cc0e7-119">Выберите поле рядом с **удалением программного обеспечения драйвера для этого устройства** и выберите **Uninstall.**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="cc0e7-120">Примечание. На данном этапе может потребоваться перезапустить компьютер.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="cc0e7-121">Перед перезапуском обязательно запишите оставшиеся инструкции.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="cc0e7-122">Откройте диспетчер устройств снова.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="cc0e7-123">**Расширите раздел Адаптеры** отображения, щелкните правой кнопкой мыши на вашем адаптере отображения и выберите **драйвер обновления.**</span><span class="sxs-lookup"><span data-stu-id="cc0e7-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="cc0e7-124">Выберите **поиск автоматически для обновления программного** обеспечения драйвера и следуйте инструкциям по установке.</span><span class="sxs-lookup"><span data-stu-id="cc0e7-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>