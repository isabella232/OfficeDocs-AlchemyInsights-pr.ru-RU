---
title: Удаление корневого сайта SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815484"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="5a7d5-102">Удаление корневого сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="5a7d5-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="5a7d5-103">Удаление корневого сайта SharePoint **не поддерживается**.</span><span class="sxs-lookup"><span data-stu-id="5a7d5-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="5a7d5-104">Если корневой сайт уже удален, при попытке получить доступ к сайту пользователи увидят сообщение об ошибке 404, "Файл не найден".</span><span class="sxs-lookup"><span data-stu-id="5a7d5-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="5a7d5-105">Чтобы устранить эту проблему, восстановите сайт в новом центре администрирования SharePoint. Для этого на странице [Удаленные сайты](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) выберите корневой сайт и нажмите кнопку "Восстановить".</span><span class="sxs-lookup"><span data-stu-id="5a7d5-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="5a7d5-106">После восстановления корневого сайта вместо того, чтобы удалять его, используйте функцию [замены сайта](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) в новом центре администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5a7d5-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="5a7d5-107">Дополнительную информацию см. в статье [Модернизация корневого сайта](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="5a7d5-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>