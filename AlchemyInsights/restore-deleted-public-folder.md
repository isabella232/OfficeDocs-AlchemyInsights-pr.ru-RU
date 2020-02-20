---
title: Восстановление удаленной общедоступной папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158536"
---
# <a name="restore-a-deleted-public-folder"></a>Восстановление удаленной общедоступной папки

**Чтобы восстановить удаленные элементы из общедоступной папки,** выполните следующие действия.

- Просмотр [удаленных элементов из общедоступной папки, отличной от почты, в Outlook 2016](https://aka.ms/pfrec).
 
**Чтобы восстановить удаленную общедоступную папку (любой тип)**, выполните указанные ниже действия. 

- Выполните следующую команду EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Пример: Следующая команда восстановит Subfolder1 и поместит ее в \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Дополнительные сведения см. [в статье Восстановление удаленной общедоступной папки](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
