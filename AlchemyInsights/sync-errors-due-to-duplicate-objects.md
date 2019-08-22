---
title: 902 (ошибки синхронизации из-за дублирования объектов)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507428"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ошибки синхронизации из-за повторяющихся объектов

При завершении синхронизации службы каталогов в Office 365 может появиться одно из следующих сообщений об ошибке:

- Не удалось обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальном каталоге.

- Синхронизированный объект с таким же прокси-адресом уже существует в вашем каталоге Microsoft Online Services.

- Не удалось обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальных службах каталогов: UserPrincipalName.

Чтобы определить и устранить проблему, скачайте и запустите [средство устранения ошибок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Дополнительные сведения см. в разделе [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
