---
title: Устранение неполадок при доступе к сообщениям
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690796"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="cfb8a-102">Устранение неполадок при доступе к сообщениям</span><span class="sxs-lookup"><span data-stu-id="cfb8a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="cfb8a-103">Если кто-то получил сообщение "отказано в доступе" к общей папке в SharePoint, администратор семейства веб-сайтов мог включить режим "ограниченный доступ пользователей".</span><span class="sxs-lookup"><span data-stu-id="cfb8a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="cfb8a-104">Чтобы отключить эту функцию, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="cfb8a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="cfb8a-105">Перейдите на сайт, щелкните значок "Параметры" и выберите пункт **Параметры сайта**.</span><span class="sxs-lookup"><span data-stu-id="cfb8a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="cfb8a-106">В разделе **Администрирование семейства веб-сайтов** щелкните **Возможности семейства веб-сайтов**.</span><span class="sxs-lookup"><span data-stu-id="cfb8a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="cfb8a-107">В **режиме ограниченный доступ пользователей к режиму блокировки**нажмите кнопку **Отключить**.</span><span class="sxs-lookup"><span data-stu-id="cfb8a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="cfb8a-108">Сообщение об отказе в доступе также может произойти для общих папок, если сайт является сайтом публикации.</span><span class="sxs-lookup"><span data-stu-id="cfb8a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="cfb8a-109">Сведения см. [в статье отказ в доступе при доступе к общей папке](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="cfb8a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="cfb8a-110">Если кто-то получил сообщение "отказано в доступе" при попытке просмотра запросов на доступ, необходимо добавить пользователя в качестве администратора семейства веб-сайтов или члена группы "владельцы" для сайта.</span><span class="sxs-lookup"><span data-stu-id="cfb8a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="cfb8a-111">Дополнительные сведения см. [в списке отказ в доступе к запросам на доступ](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="cfb8a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="cfb8a-112">Если пользователь получил сообщение "отказано в доступе" после того, как оно было удалено из локальной службы Active Directory и затем Добавлено обратно, ознакомьтесь со статьей [отказ в доступе при синхронизации учетной записи пользователя с Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="cfb8a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

