---
title: Этот сайт не может быть достигнут - ошибка при попытке получить доступ к сайту SharePoint из браузера или Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718201"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="b6a76-102">Ошибка "Этот сайт не может быть достигнута" при попытке получить доступ к сайту SharePoint из браузера или Teams</span><span class="sxs-lookup"><span data-stu-id="b6a76-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="b6a76-103">Пользователи могут получить ошибку "Этот сайт не может быть достигнут" при попытке получить доступ к сайту SharePoint из браузера или Teams.</span><span class="sxs-lookup"><span data-stu-id="b6a76-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="b6a76-104">Чтобы устранить эту проблему, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="b6a76-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="b6a76-105">Проверьте, находится ли домашняя страница в корзине или корзине второй стадии, и восстановим страницу.</span><span class="sxs-lookup"><span data-stu-id="b6a76-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="b6a76-106">**Пример прямого URL-адреса для утилизации корзины:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="b6a76-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="b6a76-107">Если домашняя страница будет окончательно удалена из корзины, создайте новую страницу сайта из библиотеки Страниц сайта и сделайте ее домашней страницей.</span><span class="sxs-lookup"><span data-stu-id="b6a76-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="b6a76-108">**Пример прямого URL-адреса:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="b6a76-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>