---
title: Добавление группы на сайт SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750533"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Проблемы при создании или группировании подключенных сайтов в SharePoint Online

При создании или повторном создании подключенного к группе сайта возникла пара распространенных проблем.

 Если вы удалили группу и подключенный сайт и хотите создать другой сайт с тем же URL-адресом, необходимо удалить предыдущий сайт без возможности восстановления.

Загрузка [командной консоли SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Более подробную информацию о начале работы с PowerShell можно узнать в статье [Начало работы с помощью командной консоли SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Удалите сайт из удаленных сайтов с помощью командлета PowerShell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Если вы создаете сайт, подключенный к группе, и получаете предупреждение о том, что уже существует еще одна группа с таким же псевдонимом, проверьте существующие группы из [центра администрирования Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Чтобы устранить эту проблему, удалите существующую группу, если она больше не нужна, или создайте сайт с другим назначенным псевдонимом.

Существуют различные способы создания и использования современных групп с SharePoint.

Вы можете подключить существующие сайты к группе Office 365. Для получения дополнительных сведений обратитесь [к разделу Подключение группы Office 365 с помощью пользователя SharePoint инетерфаце](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Чтобы создать сайт, подключенный к группе Office 365, необходимо создать сайт группы. Более подробную информацию можно узнать [в статье Создание сайта группы в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

