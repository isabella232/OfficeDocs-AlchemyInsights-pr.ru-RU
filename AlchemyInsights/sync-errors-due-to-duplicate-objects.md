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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708075"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ошибки синхронизации из-за дублирующихся объектов

Вы можете получить одно из следующих сообщений об ошибке после завершения синхронизации каталогов в Microsoft 365:

- Невозможно обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые уже могут быть связаны с другим объектом в локальном каталоге.

- Синхронизированный объект с тем же прокси-адресом уже существует в Microsoft Online Services каталоге.

- Невозможно обновить этот объект, так как следующие атрибуты, связанные с этим объектом, имеют значения, которые уже могут быть связаны с другим объектом в локальных службах каталогов: UserPrincipalName.

Чтобы определить и устранить проблему, скачайте и запустите средство исправления ошибок [IdFix DirSync.](https://github.com/Microsoft/idfix)

Дополнительные сведения см. в [kB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
