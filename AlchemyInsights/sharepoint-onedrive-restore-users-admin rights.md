---
title: Устранение неполадок Доступ отказано в сообщениях OneDrive для бизнеса сайтов
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957806"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Устранение неполадок Доступ отказано в сообщениях OneDrive для бизнеса сайтов

Эта проблема чаще всего возникает, когда пользователь удаляется и повторно создается с тем же основным именем пользователя (UPN). Новая учетная запись создается с помощью другого значения PUID (Passport Unique ID). Когда пользователь пытается получить доступ к коллекции сайтов или OneDrive, у пользователя имеется неправильный PUID. Второй сценарий включает синхронизацию каталогов с организационным подразделением Active Directory (OU). Если пользователи уже вписались в SharePoint, а затем перемещаются в другой OU и повторно SharePoint, они могут испытывать эту проблему.

1. Чтобы устранить эту проблему, необходимо восстановить исходный УИИ с помощью действий в статье [Восстановление пользователя](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)в Microsoft 365 .
2. Если вы не можете восстановить исходного пользователя, следует удалить старого пользователя с сайта OneDrive с помощью этих действий, удалите пользователя из списка [данных пользователя](). 
3. После этого можно убедиться, что у пользователя есть права администратора на [](https://docs.microsoft.com/sharepoint/manage-user-profiles) сайт OneDrive, следуя шагам по добавлению администратора для OneDrive

Дополнительные сведения об уровнях разрешений см. в статье "Понимание уровней разрешений [в SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
