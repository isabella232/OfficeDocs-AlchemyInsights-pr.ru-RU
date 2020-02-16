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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063730"
---
# <a name="restore-a-deleted-public-folder"></a>Восстановление удаленной общедоступной папки

**Чтобы восстановить удаленные элементы из общедоступной папки,** выполните следующие действия.

- Просмотр [удаленных элементов из общедоступной папки, отличной от почты, в Outlook 2016](https://aka.ms/pfrec).
 
**Чтобы восстановить удаленную общедоступную папку (любой тип)**, выполните указанные ниже действия. 

- Выполните следующую команду EXO PowerShell:

    Синтаксис:

    >$pf = Get – PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT — рекурсия |? {$_. Name — Eq "\<name_of_deleted_public_Folder"}; Set — PublicFolder $pf. Identity — путь \<, по которому будет восстановлена папка>

    Пример: Следующая команда восстановит Subfolder1 и поместит ее в \Parent1:

    >$pf = Get – PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT — рекурсия |? {$_. Name — Eq "Subfolder1"}; Set — PublicFolder $pf. Identity — Path \Parent1

Дополнительные сведения см. [в статье Восстановление удаленной общедоступной папки](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
