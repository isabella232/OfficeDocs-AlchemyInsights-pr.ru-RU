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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943388"
---
# <a name="restore-a-deleted-public-folder"></a>Восстановление удаленных общедоступных папок

**Восстановление удаленных элементов из общедоступных папок:**

- [См., что удаленные элементы](https://aka.ms/pfrec)не могут быть восстановлены из открытой папки без почты в Outlook 2016.
 
**Восстановление удаленных общедоступных папок (любого типа):** 

- Используйте следующую команду EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Пример. Следующая команда восстановит Subfolder1 и поместите ее в \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Дополнительные [сведения см. в материале Восстановление](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) удаленных общедоступных папок.
