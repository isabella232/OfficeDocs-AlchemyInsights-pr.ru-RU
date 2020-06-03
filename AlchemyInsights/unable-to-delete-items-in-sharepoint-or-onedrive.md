---
title: Не удается удалить элементы в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511989"
---
# <a name="unable-to-delete-items"></a>Не удается удалить элементы

Это может быть вызвано политиками хранения, а также отключением или исключением соответствующих удержаний, которые приводят к возникновению этой проблемы. После удаления политики хранения или удержания может потребоваться до 24 часов, чтобы изменения вступили в силу. Убедитесь, что для элемента отсутствует настройка [политики хранения](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .

Возможно, на сайте превышено ограничение размера хранилища, необходимо увеличить [квоту сайта](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) и удалить элемент.

Убедитесь, что элемент не [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) другим пользователем.

Наконец, администраторы могут использовать [шаблоны и методики SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) , которые содержат библиотеку команд PowerShell, которые позволяют выполнять сложные действия управления, такие как принудительное удаление элементов стубборн.
- [Удаление PNP файла](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Удаление папки PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Удаление элемента списка PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Удаление списка PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Удаление поля PNP (столбец)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)