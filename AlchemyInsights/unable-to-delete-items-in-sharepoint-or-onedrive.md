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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571284"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="07064-102">Не удается удалить элементы</span><span class="sxs-lookup"><span data-stu-id="07064-102">Unable to delete items</span></span>

<span data-ttu-id="07064-103">Это может быть вызвано политиками хранения, а также отключением или исключением соответствующих удержаний, которые приводят к возникновению этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="07064-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="07064-104">После удаления политики хранения или удержания может потребоваться до 24 часов, чтобы изменения вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="07064-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="07064-105">Убедитесь, что для элемента отсутствует настройка [политики хранения](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="07064-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="07064-106">Возможно, на сайте превышено ограничение размера хранилища, необходимо увеличить [квоту сайта](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) и удалить элемент.</span><span class="sxs-lookup"><span data-stu-id="07064-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="07064-107">Убедитесь, что элемент не [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="07064-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="07064-108">Наконец, администраторы могут использовать [шаблоны и методики SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) , которые содержат библиотеку команд PowerShell, которые позволяют выполнять сложные действия управления, такие как принудительное удаление элементов стубборн.</span><span class="sxs-lookup"><span data-stu-id="07064-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="07064-109">Удаление PNP файла</span><span class="sxs-lookup"><span data-stu-id="07064-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="07064-110">Удаление папки PNP</span><span class="sxs-lookup"><span data-stu-id="07064-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="07064-111">Удаление элемента списка PNP</span><span class="sxs-lookup"><span data-stu-id="07064-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="07064-112">Удаление списка PNP</span><span class="sxs-lookup"><span data-stu-id="07064-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="07064-113">Удаление поля PNP (столбец)</span><span class="sxs-lookup"><span data-stu-id="07064-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)