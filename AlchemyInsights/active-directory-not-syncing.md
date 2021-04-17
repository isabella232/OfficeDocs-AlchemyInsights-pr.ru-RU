---
title: Active Directory, не синхронизируются
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822864"
---
# <a name="active-directory-not-syncing"></a>Active Directory, не синхронизируются

Если вы получаете ошибки синхронизации, такие как "не последняя синхронизация", или обратите внимание, что состояние синхронизации каталогов на портале администрирования Office гласит: "Последняя синхронизация была выполнена более 3 дней назад", возможно, что AADConnect имеет неправильные параметры или недостаточно разрешений для выполнения синхронизации.  

Переустановка AADConnect с помощью экспресс-параметров может быстро устранить проблему:

1. [Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следуйте инструкциям по экспресс-установке.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Дополнительные сведения об учетных записях службы AADConnect см. в статье [Azure AD Connect: учетные записи и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
