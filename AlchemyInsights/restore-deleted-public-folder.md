---
title: Восстановление удаленной общедоступной папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774544"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="57334-102">Восстановление удаленной общедоступной папки</span><span class="sxs-lookup"><span data-stu-id="57334-102">Restore a deleted public folder</span></span>

<span data-ttu-id="57334-103">**Чтобы восстановить удаленные элементы из общедоступной папки,** выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="57334-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="57334-104">Просмотр [удаленных элементов из общедоступной папки, отличной от почты, в Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="57334-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="57334-105">**Чтобы восстановить удаленную общедоступную папку (любой тип)**, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="57334-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="57334-106">Выполните следующую команду EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="57334-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="57334-107">Синтаксис:</span><span class="sxs-lookup"><span data-stu-id="57334-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="57334-108">Пример: Следующая команда восстановит Subfolder1 и поместит ее в \Parent1:</span><span class="sxs-lookup"><span data-stu-id="57334-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="57334-109">Дополнительные сведения см. [в статье Восстановление удаленной общедоступной папки](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="57334-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
