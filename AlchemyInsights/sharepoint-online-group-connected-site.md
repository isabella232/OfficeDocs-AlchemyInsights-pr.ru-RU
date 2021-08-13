---
title: Добавление группы на сайт SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093723"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Распространенные проблемы при создании сайта, связанного с группой в SharePoint

1. Если вы удалили группу и связанный с ней сайт и хотите создать другой сайт с тем же URL-адресом, вам потребуется окончательно удалить предыдущий сайт.

   - Загрузка [оболочки управления SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Дополнительные сведения о том, как начать работу с Powershell, см. в SharePoint [Online Management Shell.](/powershell/module/sharepoint-online/remove-sposite)
   - Удалите сайт из удаленных сайтов с помощью [cmdlet Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell необходимо постоянно удалять сайты групп.

1. Если вы создаете сайт, подключенный к группе, и получаете **предупреждение:** другая группа с тем же псевдонимом уже существует, проверьте существующие группы из [Центр администрирования Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Чтобы устранить проблему, удалите существующую группу, если она больше не нужна, или создайте сайт с другим псевдонимом.

1. Существуют различные способы создания и использования современных групп с SharePoint.

   - Вы можете подключить существующие сайты к Microsoft 365 группе. Дополнительные сведения [см. в Подключение группе Microsoft 365 с помощью пользовательского интерфейса SharePoint.](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Чтобы создать Microsoft 365, связанный с группой, необходимо создать сайт [Team Site.](https://admin.microsoft.com/sharepoint)
