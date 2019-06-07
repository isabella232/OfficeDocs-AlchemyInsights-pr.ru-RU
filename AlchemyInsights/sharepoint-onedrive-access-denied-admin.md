---
title: Устранение неполадок при доступе к сообщениям
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760353"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Устранение неполадок в сообщениях отказа в доступе в SharePoint и в центре администрирования OneDrive

Если вы получаете сообщение об отказе в доступе при попытке перейти в центр администрирования SharePoint или OneDrive, убедитесь, что вы [назначили пользователю лицензию](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Если у пользователя есть лицензия, убедитесь, что [ей назначена роль администратора](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , которая может получать доступ к центрам администрирования.

Эта проблема также может возникать, если пользователь удален и повторно создан с тем же именем участника-пользователя (UPN). Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта). Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID. Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU). Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.

Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и [восстановить пользователя в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Примечание: Если центр администрирования OneDrive или SharePoint недоступен для нескольких пользователей, у которых ранее был доступ, может возникнуть временная ошибка службы.  [Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).


