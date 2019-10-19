---
title: Не удается удалить элементы в SharePoint или OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748589"
---
# <a name="unable-to-delete-items"></a>Не удается удалить элементы

Возникли проблемы с удалением элементов SharePoint?

- Всегда убедитесь, что у вас есть [соответствующие разрешения](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) на удаление элемента или если [администратор семейства веб-сайтов](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) попытался удалить элемент.

- Убедитесь, что для элемента отсутствует настройка [политики хранения](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

- Убедитесь, что элемент не [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) другим пользователем.

- Наконец, администраторы могут использовать [шаблоны и методики SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) , которые содержат библиотеку команд PowerShell, которые позволяют выполнять сложные действия управления, такие как принудительное удаление элементов стубборн.
- [Удаление PNP файла](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Удаление папки PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Удаление элемента списка PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Удаление списка PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Удаление поля PNP (столбец)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)