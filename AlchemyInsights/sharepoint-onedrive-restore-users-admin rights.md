---
title: Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232550"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса

Эта проблема чаще всего возникает, когда пользователь удаляется и повторно создается с тем же именем участника-пользователя (UPN). Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта). Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID. Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU). Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.

1. Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и[восстановить пользователя в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Если не удается восстановить исходного пользователя, необходимо удалить старого пользователя с сайта OneDrive, выполнив указанные ниже действия, [удалить пользователя из списка сведений о пользователе](). 
3. После этого вы можете проверить, есть ли у пользователя права администратора на сайте OneDrive, выполнив действия, описанные в статье [Добавление администратора для onedrive пользователя](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Более подробную информацию об уровнях разрешений можно узнать в статье, посвященной [уровням разрешений в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
