---
title: Открыть в проводнике не работает
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307904"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="4c3c4-102">Открыть в проводнике не работает</span><span class="sxs-lookup"><span data-stu-id="4c3c4-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="4c3c4-p101">Если не удается **Открыть в проводнике** или **представления в обозревателе файла** убедитесь, что служба веб-клиента задано значение **под управлением** , выполнив следующие действия. Например он может занять много времени, чтобы открыть библиотеку SharePoint или OneDrive, если служба не запущена.</span><span class="sxs-lookup"><span data-stu-id="4c3c4-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="4c3c4-105">В поле поиска Windows тип запуска, выберите выполнить классического приложения, введите services.msc и выберите **Ввод**.</span><span class="sxs-lookup"><span data-stu-id="4c3c4-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="4c3c4-p102">Прокрутите список вниз до службу веб-клиента и установить флажок в столбце **состояние** . Если состояние службы веб-клиента не **под управлением**, дважды щелкните имя службы, нажмите кнопку **Пуск**и затем нажмите **кнопку ОК**. Включите службу, при необходимости, выбрав в списке **Тип запуска** **вручную** или **автоматически** .</span><span class="sxs-lookup"><span data-stu-id="4c3c4-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4c3c4-p103">Для устранения неполадок, открыв в File Explorer, видеть [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665). Изучите синхронизации как лучший вариант: [файлы синхронизации SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="4c3c4-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

