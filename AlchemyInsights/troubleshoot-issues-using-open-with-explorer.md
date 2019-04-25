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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390620"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="11756-102">Устранение проблем с открытием в проводнике</span><span class="sxs-lookup"><span data-stu-id="11756-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="11756-103">Устранение распространенных проблем с открытием библиотеки документов в SharePoint или OneDrive с помощью команды " **Открыть с помощью проводника** ":</span><span class="sxs-lookup"><span data-stu-id="11756-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="11756-104">Используйте Internet Explorer 10 или Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="11756-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="11756-105">**Open With Explorer** несовместим с Microsoft EDGE, Google Chrome, Firefox и др.</span><span class="sxs-lookup"><span data-stu-id="11756-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="11756-106">Надстройка " **Открыть в проводнике** " отключена во всех браузерах, кроме Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="11756-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="11756-107">В современном интерфейсе для библиотек SharePoint недоступен режим " **Открыть с помощью проводника** ".</span><span class="sxs-lookup"><span data-stu-id="11756-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="11756-108">Используйте вместо этого **представление в проводнике** .</span><span class="sxs-lookup"><span data-stu-id="11756-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="11756-109">Выберите Просмотр **параметров** \> **в проводнике**.</span><span class="sxs-lookup"><span data-stu-id="11756-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="11756-110">Представление в проводнике не совместимо с Microsoft EDGE, Google Chrome, Firefox и т. д.</span><span class="sxs-lookup"><span data-stu-id="11756-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="11756-111">**Представление в проводнике** доступно только в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="11756-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="11756-112">Убедитесь, что служба WebClient запущена.</span><span class="sxs-lookup"><span data-stu-id="11756-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="11756-113">В поле поиска Windows введите команду Run (запустить классическое приложение), введите Services. msc и нажмите клавишу ВВОД.</span><span class="sxs-lookup"><span data-stu-id="11756-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="11756-114">ПроКрутите список вниз до службы WebClient и убедитесь, что в столбце **состояние** отображается текст "работает".</span><span class="sxs-lookup"><span data-stu-id="11756-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="11756-115">Если это не так, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="11756-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="11756-116">(Возможно, потребуется сначала включить службу, выбрав в поле **Тип запуска** значение **вручную** или **автоматически** .)</span><span class="sxs-lookup"><span data-stu-id="11756-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="11756-117">Открыть библиотеку в проводнике удобно, если вам нужно скопировать или переместить несколько файлов и папок один раз, но если вы хотите регулярно работать в библиотеке, рекомендуем синхронизировать ее.</span><span class="sxs-lookup"><span data-stu-id="11756-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="11756-118">Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="11756-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="11756-119">Сведения о настройке синхронизации можно найти в статье [Синхронизация файлов SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="11756-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="11756-120">В этой статье [описано, как использовать команду "открыть в проводнике" для устранения неполадок в SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="11756-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

