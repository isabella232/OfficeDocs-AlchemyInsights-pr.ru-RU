---
title: Невозможно удалить элементы в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038530"
---
# <a name="unable-to-delete-items"></a>Невозможно удалить элементы

- Это может привести к тому, что политика хранения может привести к отключению или исключению соответствующего удержания, что вызывает эту проблему. После удаления политики хранения или удержания изменение может занять до 24 часов. Убедитесь, что на элементе не [установлена](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) политика хранения.

- Возможно, сайт превысил ограничение на хранение, увеличил квоту [сайта](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) и удалил элемент.

- Убедитесь, что элемент не [выехав другому](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) пользователю.

- Наконец, администраторы могут [SharePoint шаблоны](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) и практики (PnP), содержащий библиотеку команд PowerShell, которые позволяют выполнять сложные действия управления, такие как принудительное удаление упорных элементов.
- [Удаление PNP-файла](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Удаление папки PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Удаление элемента списка PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Удаление списка PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Удаление поля PNP (Столбец)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)