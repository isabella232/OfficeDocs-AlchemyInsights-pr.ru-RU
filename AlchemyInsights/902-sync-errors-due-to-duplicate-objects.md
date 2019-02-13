---
title: 902 (ошибки синхронизации из-за повторяющихся объектов)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919885"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Ошибки синхронизации из-за повторяющихся объектов

Вы можете получить одно из следующих сообщений об ошибке после завершения синхронизации службы каталогов:
  
- Не удается обновить этот объект в Microsoft Online Services, так как следующие атрибуты, связанное с объектом значения, которые могут быть уже связаны с другой объект в локальный каталог.
    
- Синхронизированных объектов с тем же адресом прокси-сервер уже существует в каталоге Microsoft Online Services.
    
- Не удается обновить этот объект, так как следующие атрибуты, связанное с объектом значения, которые могут быть уже связаны с другой объект в локальный каталог служб: UserPrincipalName.
    
Чтобы определить и устранить проблему, загрузите и запустите [Средство исправления ошибок IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).
  
Для получения дополнительных сведений см [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

