---
title: Удаление корневого сайта SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768456"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="f9965-102">Удаление корневого сайта SharePoint</span><span class="sxs-lookup"><span data-stu-id="f9965-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="f9965-103">Удаление корневого сайта SharePoint **не поддерживается.**</span><span class="sxs-lookup"><span data-stu-id="f9965-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="f9965-104">Если корневой сайт уже удален, при попытке получить доступ к сайту пользователи увидят сообщение об ошибке 404, «Файл не найден».</span><span class="sxs-lookup"><span data-stu-id="f9965-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="f9965-105">Чтобы устранить эту проблему, восстановите сайт в новом центре администрирования SharePoint. Для этого на странице [Удаленные сайты](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) выберите корневой сайт и нажмите кнопку «Восстановить».</span><span class="sxs-lookup"><span data-stu-id="f9965-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="f9965-106">После восстановления корневого сайта впредь, вместо того чтобы удалять его, используйте функцию [замены сайта](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) в новом центре администрирования SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f9965-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="f9965-107">Дополнительную информацию см. в статье [Модернизация корневого сайта](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="f9965-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>