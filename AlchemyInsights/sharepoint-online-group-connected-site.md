---
title: Добавление группы на сайт SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770364"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблемы при создании сайта с подключением к группе в SharePoint

1. Некоторые распространенные проблемы, возникающие при создании или повторном создании подключенного к группе сайта.
Если вы удалили группу и подключенный сайт и хотите создать другой сайт с тем же URL-адресом, необходимо удалить предыдущий сайт без возможности восстановления.

   - Загрузка [командной консоли SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Более подробную информацию о начале работы с PowerShell можно узнать в статье [Начало работы с консолью управления SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Удалите сайт из удаленных сайтов с помощью командлета PowerShell [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . Для окончательного удаления групп сайтов требуется PowerShell.

1. Если вы создаете сайт, подключенный к группе, и получаете предупреждение: **уже существует другая группа с таким же псевдонимом**, проверьте существующие группы из [центра администрирования Office 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Чтобы устранить эту проблему, удалите существующую группу, если она больше не нужна, или создайте сайт с другим назначенным псевдонимом.

1. Существуют различные способы создания и использования современных групп с SharePoint.

   - Вы можете подключить существующие сайты к группе Office 365. Для получения дополнительных сведений обратитесь [к разделу Подключение группы Office 365 с помощью пользовательского интерфейса SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Чтобы создать сайт, подключенный к группе Office 365, необходимо создать [сайт группы](https://admin.microsoft.com/sharepoint).
