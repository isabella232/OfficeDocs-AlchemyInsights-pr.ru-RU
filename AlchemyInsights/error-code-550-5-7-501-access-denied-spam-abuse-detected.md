---
title: Код ошибки 550 5.7.501 отказано в доступе, обнаружена Нежелательная почта
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36740154"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="2c3c5-102">550 5.7.501 отказано в доступе, обнаружена Нежелательная почта</span><span class="sxs-lookup"><span data-stu-id="2c3c5-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="2c3c5-103">Как правило, это сообщение появляется, когда пользователи отправляют сообщения электронной почты с IP-адресов с помощью начального домена *onmicrosoft.com* , назначенного новым клиентам в Office 365.</span><span class="sxs-lookup"><span data-stu-id="2c3c5-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="2c3c5-104">Самый простой способ устранить эту проблему:</span><span class="sxs-lookup"><span data-stu-id="2c3c5-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="2c3c5-105">[Добавление домена в клиент](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="2c3c5-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="2c3c5-106">[Измените основной адрес электронной почты пользователя](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) на новый личный домен, который вы только что добавили.</span><span class="sxs-lookup"><span data-stu-id="2c3c5-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
