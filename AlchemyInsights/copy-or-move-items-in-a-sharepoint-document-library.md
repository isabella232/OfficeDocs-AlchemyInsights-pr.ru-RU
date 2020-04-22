---
title: Копирование или перемещение элементов в библиотеке документов SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: b8324f596b6830998bb7e659d561a015a7ba2b1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715681"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="ce52f-102">Копирование или перемещение элементов в библиотеке документов SharePoint</span><span class="sxs-lookup"><span data-stu-id="ce52f-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="ce52f-103">Можно копировать и перемещать файлы, папки и ссылки на различные расположения в библиотеке документов.</span><span class="sxs-lookup"><span data-stu-id="ce52f-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="ce52f-104">Вы также можете копировать элементы на сайтах.</span><span class="sxs-lookup"><span data-stu-id="ce52f-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="ce52f-105">В браузере перейдите к файлам, папкам или ссылкам, которые требуется переместить, а затем нажмите кнопку **Копировать в** или **переместить**.</span><span class="sxs-lookup"><span data-stu-id="ce52f-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ce52f-106">" **Копировать** " и " **переместить** " недоступно, если вы используете классический интерфейс SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ce52f-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="ce52f-107">В разделе **Выбор назначения**выберите расположение, в которое вы хотите скопировать или переместить элементы, или нажмите кнопку **Обзор сайтов** , чтобы просмотреть полный список сайтов.</span><span class="sxs-lookup"><span data-stu-id="ce52f-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ce52f-108">Если вы не видите другие сайты, указанные при копировании элементов, копирование между сайтами не было настроено.</span><span class="sxs-lookup"><span data-stu-id="ce52f-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="ce52f-109">Чтобы включить его, перейдите на страницу параметров центра администрирования SharePoint и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ce52f-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="ce52f-110">Чтобы создать новую папку, выберите расположение в иерархии папок, щелкните **создать папку**, введите имя папки и установите флажок, чтобы сохранить имя.</span><span class="sxs-lookup"><span data-stu-id="ce52f-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="ce52f-111">Щелкните **Копировать здесь** или **Переместите здесь**.</span><span class="sxs-lookup"><span data-stu-id="ce52f-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ce52f-112">Вы можете одновременно скопировать до 500 МБ файлов и папок.</span><span class="sxs-lookup"><span data-stu-id="ce52f-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="ce52f-113">> при копировании документов с журналом версий копируется только последняя версия.</span><span class="sxs-lookup"><span data-stu-id="ce52f-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="ce52f-114">При перемещении документов их журнал также перемещается.</span><span class="sxs-lookup"><span data-stu-id="ce52f-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="ce52f-115">При перемещении файла он по-прежнему будет отображаться в исходном каталоге, пока он не будет полностью перемещен в место назначения, а затем будет удален.</span><span class="sxs-lookup"><span data-stu-id="ce52f-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="ce52f-116">Файл останется в корзине исходного сайта после завершения перемещения и будет подчиняться нормальному расписанию повторного запуска, если пользователь не восстанавливает его из корзины.</span><span class="sxs-lookup"><span data-stu-id="ce52f-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="ce52f-117">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="ce52f-117">For more information, see:</span></span>

 - <span data-ttu-id="ce52f-118">[Перемещение и копирование файлов в SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (статья о службе поддержки Office)</span><span class="sxs-lookup"><span data-stu-id="ce52f-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="ce52f-119">[Перемещение файлов из любой папки](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (статья блога технического сообщества Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce52f-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  