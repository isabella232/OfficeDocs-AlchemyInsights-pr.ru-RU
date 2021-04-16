---
title: Восстановление удаленных общедоступных папок
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809452"
---
# <a name="restore-a-deleted-public-folder"></a>Восстановление удаленных общедоступных папок

**Восстановление удаленных элементов из общедоступных папок:**

- См. статью Вы не можете восстановить удаленные элементы из открытой папки без почты [в Outlook 2016](https://aka.ms/pfrec).
 
**Восстановление удаленных общедоступных папок (любого типа):** 

- Используйте следующую команду EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Пример. Следующая команда восстановит Subfolder1 и поместите ее в \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Дополнительные [сведения см. в материале Восстановление](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) удаленных общедоступных папок.
