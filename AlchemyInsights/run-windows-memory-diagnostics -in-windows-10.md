---
title: Запуск диагностики памяти Windows в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289808"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="236a1-102">Запуск диагностики памяти Windows в Windows 10</span><span class="sxs-lookup"><span data-stu-id="236a1-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="236a1-103">Если Windows и приложения на компьютере дают сбой, зависают или работают неустойчиво, возможно, у вас возникла проблема с памятью компьютера (ОЗУ).</span><span class="sxs-lookup"><span data-stu-id="236a1-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="236a1-104">Вы можете запустить диагностику памяти Windows, чтобы проверить, есть ли у компьютера проблемы с ОЗУ.</span><span class="sxs-lookup"><span data-stu-id="236a1-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="236a1-105">В поле поиска на панели задач введите **Диагностика памяти**, а затем выберите **Диагностика памяти Windows**.</span><span class="sxs-lookup"><span data-stu-id="236a1-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="236a1-106">Чтобы запустить диагностику, компьютер необходимо перезапустить.</span><span class="sxs-lookup"><span data-stu-id="236a1-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="236a1-107">Вы можете перезагрузить компьютер немедленно (сначала сохраните свою работу и закройте открытые документы и сообщения электронной почты) или запланировать автоматический запуск диагностики при следующей перезагрузке компьютера.</span><span class="sxs-lookup"><span data-stu-id="236a1-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Диагностика памяти Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="236a1-109">Когда компьютер перезагрузится, **Средство диагностики памяти Windows** запустится автоматически.</span><span class="sxs-lookup"><span data-stu-id="236a1-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="236a1-110">В процессе диагностики будет отображаться ее состояние и ход выполнения. Отменить диагностику можно, нажав на клавиатуре клавишу **ESC**.</span><span class="sxs-lookup"><span data-stu-id="236a1-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="236a1-111">По завершении диагностики Windows запускается в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="236a1-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="236a1-112">Сразу после перезапуска, когда отобразится рабочий стол, рядом со значком **Центр уведомлений** на панели задач появится уведомление о том, были ли найдены ошибки в памяти.</span><span class="sxs-lookup"><span data-stu-id="236a1-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="236a1-113">Например:</span><span class="sxs-lookup"><span data-stu-id="236a1-113">For example:</span></span>

<span data-ttu-id="236a1-114">Это значок Центра уведомлений:</span><span class="sxs-lookup"><span data-stu-id="236a1-114">Here's the Action Center icon:</span></span> ![Значок Центра уведомлений](media/action-center-icon.png) 

<span data-ttu-id="236a1-116">Пример уведомления:</span><span class="sxs-lookup"><span data-stu-id="236a1-116">And a sample notification:</span></span> ![Ошибки памяти не обнаружены](media/no-memory-errors.png)

<span data-ttu-id="236a1-118">Если вы пропустили уведомление, можно выбрать значок **Центр уведомлений** на панели задач, чтобы вывести на экран **Центр уведомлений** и просмотреть прокручиваемый список уведомлений.</span><span class="sxs-lookup"><span data-stu-id="236a1-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="236a1-119">Чтобы ознакомиться с подробными сведениями, в поле поиска на панели задач введите **событие** и выберите **Просмотр событий**.</span><span class="sxs-lookup"><span data-stu-id="236a1-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="236a1-120">В левой панели \*\*Просмотра событий \*\* перейдите в раздел **Журналы Windows > Система**.</span><span class="sxs-lookup"><span data-stu-id="236a1-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="236a1-121">В правой панели прокрутите список вниз, пока в столбце **Источник** не появятся события со значением **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="236a1-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="236a1-122">Выделите каждое такое событие и ознакомьтесь со сведениями в поле вкладки **Общие**, расположенной под списком.</span><span class="sxs-lookup"><span data-stu-id="236a1-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
