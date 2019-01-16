---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308694"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b8441-102">Ограничение доступа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8441-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b8441-p101">В SharePoint и OneDrive ограничить доступ к элементам, таким как файлов, папок и списков, предоставляя доступ только к группам или отдельным пользователям, которые должны иметь доступ. По умолчанию разрешения в SharePoint, наследуются от выше в иерархии. Поэтому файл наследует разрешения из папки, который наследует разрешения из библиотеки, который наследует разрешения от сайта.</span><span class="sxs-lookup"><span data-stu-id="b8441-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b8441-p102">Могут совместно использовать более высокого уровня (например, общий доступ к весь сайт) и затем нарушение наследования, если вы не хотите общий доступ к элементам на сайте. Тем не менее мы не рекомендуем так, как оно делает обслуживание разрешения более сложных и некоторая путаница в будущем. Вот что можно сделать вместо этого:</span><span class="sxs-lookup"><span data-stu-id="b8441-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b8441-109">Если, например, которые должны видеть все содержимое папки, за исключением одного файла в нем, переместите этот файл в новое расположение, не являющихся общими.</span><span class="sxs-lookup"><span data-stu-id="b8441-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b8441-110">Если у вас есть два вложенных папок в папке, и вы хотите совместно использовать один вложенной папке с группами A и B и доступ только группа A второй вложенную папку, общий доступ к папке с группой A и добавление группы B первого вложенную папку.</span><span class="sxs-lookup"><span data-stu-id="b8441-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b8441-111">Прекращение общего доступа к файла или папки</span><span class="sxs-lookup"><span data-stu-id="b8441-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

