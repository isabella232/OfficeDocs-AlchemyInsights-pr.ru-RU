---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720695"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f804f-102">Ограничение доступа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="f804f-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f804f-103">В SharePoint и OneDrive можно ограничить доступ к элементам, например файлам, папкам и спискам, предоставив доступ только к тем группам или лицам, к которым вы хотите получить доступ.</span><span class="sxs-lookup"><span data-stu-id="f804f-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="f804f-104">По умолчанию разрешения в SharePoint наследуются выше в иерархии.</span><span class="sxs-lookup"><span data-stu-id="f804f-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="f804f-105">Таким образом, файл наследует разрешения из папки, которая наследует разрешения из библиотеки, которая наследует свои разрешения от сайта.</span><span class="sxs-lookup"><span data-stu-id="f804f-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f804f-106">Вы можете предоставить общий доступ на более высоком уровне (например, с помощью общего доступа ко всему сайту), а затем разорывать наследование, если вы не хотите предоставлять общий доступ ко всем элементам сайта.</span><span class="sxs-lookup"><span data-stu-id="f804f-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="f804f-107">Однако это не рекомендуется, так как он делает разрешения более сложными и запутанными в будущем.</span><span class="sxs-lookup"><span data-stu-id="f804f-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="f804f-108">Вместо этого можно использовать следующие действия:</span><span class="sxs-lookup"><span data-stu-id="f804f-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f804f-109">Если, например, требуется предоставить общий доступ ко всему содержимому папки, кроме одного файла, переместите этот файл в новое расположение, которое не является общим.</span><span class="sxs-lookup"><span data-stu-id="f804f-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f804f-110">Если в папке есть две подпапки, и вы хотите поделиться одной вложенной папкой с группами A и B и разрешить доступ только к второй вложенной папке, поделитесь родительской папкой Group A и добавьте группу B в первую подпапку.</span><span class="sxs-lookup"><span data-stu-id="f804f-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f804f-111">Отмена общего доступа к файлу или папке </span><span class="sxs-lookup"><span data-stu-id="f804f-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

