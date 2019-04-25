---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383884"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="28fc2-102">Ограничение доступа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="28fc2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="28fc2-103">В SharePoint и OneDrive можно ограничить доступ к элементам, например файлам, папкам и спискам, предоставив доступ только к тем группам или лицам, к которым вы хотите получить доступ.</span><span class="sxs-lookup"><span data-stu-id="28fc2-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="28fc2-104">По умолчанию разрешения в SharePoint наследуются выше в иерархии.</span><span class="sxs-lookup"><span data-stu-id="28fc2-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="28fc2-105">Таким образом, файл наследует разрешения из папки, которая наследует разрешения из библиотеки, которая наследует свои разрешения от сайта.</span><span class="sxs-lookup"><span data-stu-id="28fc2-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="28fc2-106">Вы можете предоставить общий доступ на более высоком уровне (например, с помощью общего доступа ко всему сайту), а затем разорывать наследование, если вы не хотите предоставлять общий доступ ко всем элементам сайта.</span><span class="sxs-lookup"><span data-stu-id="28fc2-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="28fc2-107">Однако это не рекомендуется, так как он делает разрешения более сложными и запутанными в будущем.</span><span class="sxs-lookup"><span data-stu-id="28fc2-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="28fc2-108">Вместо этого можно использовать следующие действия:</span><span class="sxs-lookup"><span data-stu-id="28fc2-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="28fc2-109">Если, например, требуется предоставить общий доступ ко всему содержимому папки, кроме одного файла, переместите этот файл в новое расположение, которое не является общим.</span><span class="sxs-lookup"><span data-stu-id="28fc2-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="28fc2-110">Если в папке есть две подпапки, и вы хотите поделиться одной вложенной папкой с группами A и B и разрешить доступ только к второй вложенной папке, поделитесь родительской папкой Group A и добавьте группу B в первую подпапку.</span><span class="sxs-lookup"><span data-stu-id="28fc2-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="28fc2-111">Отмена общего доступа к файлу или папке</span><span class="sxs-lookup"><span data-stu-id="28fc2-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

