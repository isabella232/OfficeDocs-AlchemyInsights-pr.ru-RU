---
title: Устранение неполадок при доступе к сообщениям
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505392"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Устранение неполадок в сообщениях отказа в доступе в SharePoint и в центре администрирования OneDrive

Если вы получаете сообщение об отказе в доступе при попытке перейти в центр администрирования SharePoint или OneDrive, убедитесь, что вы [назначили пользователю лицензию](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Если у пользователя есть лицензия, убедитесь, что [ей назначена роль администратора](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , которая может получать доступ к центрам администрирования.

Эта проблема также может возникать, если пользователь удален и повторно создан с тем же именем участника-пользователя (UPN). Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта). Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID. Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU). Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.

Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и [восстановить пользователя в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Примечание: Если центр администрирования OneDrive или SharePoint недоступен для нескольких пользователей, у которых ранее был доступ, может возникнуть временная ошибка службы.  [Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).


