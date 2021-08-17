---
title: Устранение неполадок в доступе, отказано в сообщениях
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085241"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Устранение неполадок в доступе, отказано в сообщениях в Центре администрирования Sharepoint/OneDrive

Если при попытке просмотра в Центре администрирования Sharepoint/OneDrive доступу вам отказано в доступе, убедитесь, что вы назначите пользователю [лицензию.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Если у пользователя есть лицензия, необходимо [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) также убедиться, что им назначена роль администратора, которая может получить доступ к центрам администрирования.

Эта проблема также может возникать, когда пользователь удаляется и повторно создается с тем же основным именем пользователя (UPN). Новая учетная запись создается с помощью другого значения PUID (Passport Unique ID). Когда пользователь пытается получить доступ к коллекции сайтов или OneDrive, у пользователя имеется неправильный PUID. Второй сценарий включает синхронизацию каталогов с организационным подразделением Active Directory (OU). Если пользователи уже вписались в SharePoint, а затем перемещаются в другой OU и повторно SharePoint, они могут испытывать эту проблему.

Чтобы устранить эту проблему, необходимо восстановить исходный upN с помощью действий в статье Восстановление пользователя в [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Примечание. Если центр OneDrive или SharePoint администратора не доступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная проблема с обслуживанием.  [Проверьте панель мониторинга состояния службы.](https://portal.office.com/adminportal/home#/servicehealth)


