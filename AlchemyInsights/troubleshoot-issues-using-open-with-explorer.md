---
title: Устранение неполадок с помощью команды "открыть в проводнике"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742746"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="2c239-102">Устранение проблем с открытием в проводнике</span><span class="sxs-lookup"><span data-stu-id="2c239-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="2c239-103">Устранение распространенных проблем с открытием библиотеки документов в SharePoint или OneDrive с помощью команды " **Открыть с помощью проводника** ":</span><span class="sxs-lookup"><span data-stu-id="2c239-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="2c239-104">Используйте Internet Explorer 10 или Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="2c239-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="2c239-105">**Open With Explorer** несовместим с Microsoft EDGE, Google Chrome, Firefox и др.</span><span class="sxs-lookup"><span data-stu-id="2c239-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2c239-106">Надстройка " **Открыть в проводнике** " отключена во всех браузерах, кроме Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2c239-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="2c239-107">В современном интерфейсе для библиотек SharePoint недоступен режим " **Открыть с помощью проводника** ".</span><span class="sxs-lookup"><span data-stu-id="2c239-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="2c239-108">Используйте вместо этого **представление в проводнике** .</span><span class="sxs-lookup"><span data-stu-id="2c239-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="2c239-109">Выберите Просмотр **параметров** \> **в проводнике**.</span><span class="sxs-lookup"><span data-stu-id="2c239-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="2c239-110">Представление в проводнике не совместимо с Microsoft EDGE, Google Chrome, Firefox и т. д.</span><span class="sxs-lookup"><span data-stu-id="2c239-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2c239-111">**Представление в проводнике** доступно только в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2c239-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="2c239-112">Убедитесь, что служба WebClient запущена.</span><span class="sxs-lookup"><span data-stu-id="2c239-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="2c239-113">В поле поиска Windows введите команду Run (запустить классическое приложение), введите Services. msc и нажмите клавишу ВВОД.</span><span class="sxs-lookup"><span data-stu-id="2c239-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="2c239-114">Прокрутите список вниз до службы WebClient и убедитесь, что в столбце **состояние** отображается текст "работает".</span><span class="sxs-lookup"><span data-stu-id="2c239-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="2c239-115">Если это не так, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="2c239-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2c239-116">(Возможно, потребуется сначала включить службу, выбрав в поле **Тип запуска** значение **вручную** или **автоматически** .)</span><span class="sxs-lookup"><span data-stu-id="2c239-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2c239-117">Открыть библиотеку в проводнике удобно, если вам нужно скопировать или переместить несколько файлов и папок один раз, но если вы хотите регулярно работать в библиотеке, рекомендуем синхронизировать ее.</span><span class="sxs-lookup"><span data-stu-id="2c239-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="2c239-118">Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2c239-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2c239-119">Сведения о настройке синхронизации можно найти в статье [Синхронизация файлов SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2c239-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="2c239-120">В этой статье [описано, как использовать команду "открыть в проводнике" для устранения неполадок в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="2c239-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

