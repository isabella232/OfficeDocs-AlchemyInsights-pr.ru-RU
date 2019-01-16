---
title: 902 (ошибки синхронизации из-за повторяющихся объектов)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308842"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ошибки синхронизации из-за повторяющихся объектов

Вы можете получить одно из следующих сообщений об ошибке после завершения синхронизации службы каталогов:
  
- Не удается обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанное с объектом значения, которые могут быть уже связаны с другой объект в локальный каталог.
    
- Синхронизированных объектов с тем же адресом прокси-сервер уже существует в каталоге Microsoft Online Services.
    
- Не удается обновить этот объект, так как следующие атрибуты, связанное с объектом значения, которые могут быть уже связаны с другой объект в локальный каталог служб: UserPrincipalName.
    
Чтобы определить и устранить проблему, загрузите и запустите [Средство исправления ошибок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).
  
Для получения дополнительных сведений см [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

