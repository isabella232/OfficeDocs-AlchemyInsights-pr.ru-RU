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
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771734"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Навсегда удалить сайт в SharePoint

Чтобы повторно использовать URL-адрес на удаленном сайте (чтобы повторно создать сайт) или окончательно удалить сайт, так как он больше не используется, можно использовать **окончательно удалить** из нового центра администрирования SharePoint. 

1. Перейдите на страницу [Удаленные сайты нового центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) и войдите в систему, используя учетную запись с правами администратора вашей организации. 

2. В левом столбце выберите сайт. 

3. Нажмите кнопку **окончательно удалить**. 

**Примечание**: сайты, подключенные к группе, нельзя удалить из Центра администрирования SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) необходимо будет использовать вместо этого.  

Для получения дополнительной информации см. [Окончательно удалить сайт](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
