---
title: Удаление сайта SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/24/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c060815d-1d3f-4a13-81c2-0377bbeda202
ms.openlocfilehash: f6ee16a20f2280ba4d8d28ab3fdb4672cd9963b5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927589"
---
# <a name="delete-a-sharepoint-site"></a>Удаление сайта SharePoint
 **Удаление сайтов в центре администрирования SharePoint**
  
Удаление активного сайта, перейдите в текущем Центр администрирования SharePoint, нажмите кнопку «Попробуйте прямо сейчас» в правом верхнем углу. Выберите **сайты Active**, выберите сайт и выберите команду **Удалить**. [Просмотр и восстановления удаленных сайтов в центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)выберите **удаленных сайтов**. Дополнительные сведения в разделе [Управление узлами в центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).
  
**Важные:** Если узел является частью политику хранения, не можно удалить ее, пока сайт не будет удалено из [безопасности &amp; Центр администрирования соответствия](https://protection.office.com/?rfr=AdminCenter#/homepage). Дополнительные сведения в разделе [Обзор политик хранения](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) . 
  
Советы по:
- Глобальные "Администраторы" и "Администраторы SharePoint" теперь удаление веб-сайтов, относящихся к **Office 365 группы**. Это приведет к удалению группы и всех его ресурсов, включая почтовый ящик Outlook и календарь и все каналы группами. Дополнительные сведения см.в [Удаление сайта SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- Для восстановления удаленных сайтов для 93 дней. Обратите внимание на то, что в течение 30 дней, необходимо восстанавливать удаленные группы. Дополнительные сведения см в [представление и восстановления удаленных сайтов](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).
- Чтобы полностью удалить сайт с помощью Powershell, см в примере командлет [Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) . 
  

