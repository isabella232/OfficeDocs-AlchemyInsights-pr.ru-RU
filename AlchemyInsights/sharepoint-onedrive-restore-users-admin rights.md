---
title: Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692814"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса

Эта проблема чаще всего возникает, когда пользователь удаляется и повторно создается с тем же именем участника-пользователя (UPN). Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта). Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID. Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU). Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.

1. Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и [восстановить пользователя в Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Если не удается восстановить исходного пользователя, необходимо удалить старого пользователя с сайта OneDrive, выполнив указанные ниже действия, [удалить пользователя из списка сведений о пользователе](). 
3. После этого вы можете проверить, есть ли у пользователя права администратора на сайте OneDrive, выполнив действия, описанные в статье [Добавление администратора для onedrive пользователя](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Более подробную информацию об уровнях разрешений можно узнать в статье, посвященной [уровням разрешений в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
