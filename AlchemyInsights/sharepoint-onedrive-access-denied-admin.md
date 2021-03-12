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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707967"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Устранение неполадок с отказом в доступе к сообщениям в Центре администрирования Sharepoint/OneDrive

Если при попытке просмотра в Центре администрирования Sharepoint/OneDrive вы получаете сообщение об отказе в доступе, убедитесь, что вы назначите пользователю [лицензию.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Если у пользователя есть лицензия, необходимо [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) также убедиться, что им назначена роль администратора, которая может получить доступ к центрам администрирования.

Эта проблема также может возникать, когда пользователь удаляется и повторно создается с тем же основным именем пользователя (UPN). Новая учетная запись создается с помощью другого значения PUID (Passport Unique ID). Когда пользователь пытается получить доступ к коллекции сайтов или к oneDrive, у пользователя имеется неправильный PUID. Второй сценарий включает синхронизацию каталогов с организационным подразделением Active Directory (OU). Если пользователи уже подписались на SharePoint, а затем перемещаются в другой OU и повторно с SharePoint, у них может возникнуть эта проблема.

Чтобы устранить эту проблему, необходимо восстановить исходный upN с помощью действий в статье [Восстановление пользователя в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Примечание. Если центр администрирования OneDrive или SharePoint не доступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная проблема с обслуживанием.  [Проверьте панель мониторинга состояния службы.](https://portal.office.com/adminportal/home#/servicehealth)


