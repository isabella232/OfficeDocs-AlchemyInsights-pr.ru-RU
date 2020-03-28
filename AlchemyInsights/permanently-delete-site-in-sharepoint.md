---
title: Навсегда удалить сайт в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955240"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Навсегда удалить сайт в SharePoint

Чтобы повторно использовать URL-адрес на удаленном сайте (чтобы повторно создать сайт) или окончательно удалить сайт, так как он больше не используется, можно использовать **окончательно удалить** из нового центра администрирования SharePoint. 

1. Перейдите на страницу [Удаленные сайты нового центра администрирования SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) и войдите в систему, используя учетную запись с правами администратора вашей организации. 

2. В левом столбце выберите сайт. 

3. Нажмите кнопку **окончательно удалить**. 

**Примечание**: сайты, подключенные к группе, нельзя удалить из Центра администрирования SharePoint. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) необходимо будет использовать вместо этого.  

Для получения дополнительной информации см. [Окончательно удалить сайт](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
