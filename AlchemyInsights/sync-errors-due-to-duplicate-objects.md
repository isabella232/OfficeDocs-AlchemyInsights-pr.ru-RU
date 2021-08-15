---
title: 902 (Ошибки синхронизации из-за дублирующихся объектов)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998807"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ошибки синхронизации из-за дублирующихся объектов

Вы можете получить одно из следующих сообщений об ошибке, когда синхронизация каталогов завершится в Microsoft 365:

- Невозможно обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые уже могут быть связаны с другим объектом в локальном каталоге.

- Синхронизированный объект с тем же прокси-адресом уже существует в Microsoft Online Services каталоге.

- Невозможно обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые уже могут быть связаны с другим объектом в локальных службах каталогов: UserPrincipalName.

Чтобы определить и устранить проблему, скачайте и запустите средство исправления ошибок [IdFix DirSync.](https://github.com/Microsoft/idfix)

Дополнительные сведения см. в [kB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
