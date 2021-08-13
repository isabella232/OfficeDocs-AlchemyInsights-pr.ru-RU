---
title: Навсегда удалить сайт в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944324"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Навсегда удалить сайт в SharePoint

Чтобы повторно использовать URL-адрес на удаленном сайте (чтобы повторно создать сайт) или окончательно удалить сайт, так как он больше не используется, можно использовать **окончательно удалить** из нового центра администрирования SharePoint. 

1. Перейдите на страницу [Удаленные сайты нового центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) и войдите в систему, используя учетную запись с правами администратора вашей организации. 

2. В левом столбце выберите сайт. 

3. Нажмите кнопку **окончательно удалить**. 

**Примечание**: сайты, подключенные к группе, нельзя удалить из Центра администрирования SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) необходимо будет использовать вместо этого.  

Для получения дополнительной информации см. [Окончательно удалить сайт](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
