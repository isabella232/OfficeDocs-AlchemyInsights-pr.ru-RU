---
title: В Windows 10 отсутствует значок питания или батареи
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790561"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="809c9-102">В Windows 10 отсутствует значок питания или батареи</span><span class="sxs-lookup"><span data-stu-id="809c9-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="809c9-103">Если на устройстве с Windows 10 есть батарея (например, ноутбук, планшет или компьютер, подключенный по USB к ИБП), на панели задач рядом с часами обычно отображается значок питания или батареи. Например:</span><span class="sxs-lookup"><span data-stu-id="809c9-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Значок батареи](media/battery-icon.png)

<span data-ttu-id="809c9-105">Если вы не видите этот значок, он может быть скрыт:</span><span class="sxs-lookup"><span data-stu-id="809c9-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="809c9-106">Выберите **[Параметры > Персонализация > Панель задач](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="809c9-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="809c9-107">В области уведомлений щелкните **Выберите значки, отображаемые в панели задач**.</span><span class="sxs-lookup"><span data-stu-id="809c9-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="809c9-108">Затем найдите элемент **Питание** в списке и переведите его переключатель в положение **Вкл**.</span><span class="sxs-lookup"><span data-stu-id="809c9-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Отображение значка питания на панели задач](media/power-icon-on.png)

<span data-ttu-id="809c9-110">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="809c9-110">**Troubleshooting**</span></span>

<span data-ttu-id="809c9-111">Если при выполнении вышеуказанных инструкций переключатель **Питание** затенен или не виден, в поле поиска на панели задач введите **диспетчер устройств** и выберите **Диспетчер устройств** в списке результатов.</span><span class="sxs-lookup"><span data-stu-id="809c9-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="809c9-112">В разделе **Батареи** щелкните правой кнопкой мыши батарею своего устройства, выберите **Отключить** и щелкните **Да**.</span><span class="sxs-lookup"><span data-stu-id="809c9-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="809c9-113">Подождите несколько секунд, щелкните правой кнопкой мыши батарею и выберите **Включить**.</span><span class="sxs-lookup"><span data-stu-id="809c9-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="809c9-114">Перезагрузите устройство.</span><span class="sxs-lookup"><span data-stu-id="809c9-114">Then restart your device.</span></span>

<span data-ttu-id="809c9-115">Если вы выполнили вышеуказанные инструкции, но значок батареи не отображается на панели задач, в поле поиска на панели задач введите **диспетчер задач** и щелкните **Диспетчер задач** в списке результатов.</span><span class="sxs-lookup"><span data-stu-id="809c9-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="809c9-116">На вкладке **Процессы** в столбце **Имя** щелкните правой кнопкой мыши **Проводник** и нажмите **Перезапустить**.</span><span class="sxs-lookup"><span data-stu-id="809c9-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
