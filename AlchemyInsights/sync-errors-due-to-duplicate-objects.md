---
title: 902 (ошибки синхронизации из-за дублирования объектов)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767148"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ошибки синхронизации из-за повторяющихся объектов

При завершении синхронизации службы каталогов в Microsoft 365 может появиться одно из следующих сообщений об ошибке:

- Не удалось обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальном каталоге.

- Синхронизированный объект с таким же прокси-адресом уже существует в вашем каталоге Microsoft Online Services.

- Не удалось обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые могут быть уже связаны с другим объектом в локальных службах каталогов: UserPrincipalName.

Чтобы определить и устранить проблему, скачайте и запустите [средство устранения ошибок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Дополнительные сведения см. в разделе [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
