---
title: Открытие с помощью проводника не работает
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764921"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="49481-102">Открытие с помощью проводника не работает</span><span class="sxs-lookup"><span data-stu-id="49481-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="49481-103">Если **окно Открыть в проводнике** или **Просмотреть в проводнике** не работает, убедитесь, что служба WebClient настроена на **Запуск** , выполнив указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="49481-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="49481-104">Например, для открытия библиотеки SharePoint или OneDrive может потребоваться много времени, если служба не запущена.</span><span class="sxs-lookup"><span data-stu-id="49481-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="49481-105">В поле поиска Windows введите выполнить, выберите классическое приложение Run. msc, введите Services. msc и нажмите клавишу **Ввод**.</span><span class="sxs-lookup"><span data-stu-id="49481-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="49481-106">ПроКрутите список вниз до службы WebClient и проверьте столбец **состояние** .</span><span class="sxs-lookup"><span data-stu-id="49481-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="49481-107">Если служба WebClient не **запущена**, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="49481-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="49481-108">Включите службу (при необходимости), выбрав в поле **Тип запуска** значение **вручную** или **автоматически** .</span><span class="sxs-lookup"><span data-stu-id="49481-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="49481-109">Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="49481-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="49481-110">Узнайте, как лучше всего синхронизировать [файлы SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="49481-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

