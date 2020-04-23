---
title: Устранение неполадок при доступе к сообщениям
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759813"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="1f8f0-102">Устранение неполадок при доступе к сообщениям</span><span class="sxs-lookup"><span data-stu-id="1f8f0-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="1f8f0-103">Если кто-то получил сообщение "отказано в доступе" к общей папке в SharePoint, администратор семейства веб-сайтов мог включить режим "ограниченный доступ пользователей".</span><span class="sxs-lookup"><span data-stu-id="1f8f0-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="1f8f0-104">Чтобы отключить эту функцию, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="1f8f0-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="1f8f0-105">Перейдите на сайт, щелкните значок "Параметры" и выберите пункт **Параметры сайта**.</span><span class="sxs-lookup"><span data-stu-id="1f8f0-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="1f8f0-106">В разделе **Администрирование семейства веб-сайтов** щелкните **Возможности семейства веб-сайтов**.</span><span class="sxs-lookup"><span data-stu-id="1f8f0-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="1f8f0-107">В **режиме ограниченный доступ пользователей к режиму блокировки**нажмите кнопку **Отключить**.</span><span class="sxs-lookup"><span data-stu-id="1f8f0-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="1f8f0-108">Сообщение об отказе в доступе также может произойти для общих папок, если сайт является сайтом публикации.</span><span class="sxs-lookup"><span data-stu-id="1f8f0-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="1f8f0-109">Сведения см. [в статье отказ в доступе при доступе к общей папке](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="1f8f0-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="1f8f0-110">Если кто-то получил сообщение "отказано в доступе" при попытке просмотра запросов на доступ, необходимо добавить пользователя в качестве администратора семейства веб-сайтов или члена группы "владельцы" для сайта.</span><span class="sxs-lookup"><span data-stu-id="1f8f0-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="1f8f0-111">Дополнительные сведения см. [в списке отказ в доступе к запросам на доступ](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="1f8f0-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="1f8f0-112">Если пользователь получил сообщение "отказано в доступе" после того, как оно было удалено из локальной службы Active Directory и затем Добавлено обратно, ознакомьтесь со статьей [отказ в доступе при синхронизации учетной записи пользователя с Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="1f8f0-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

