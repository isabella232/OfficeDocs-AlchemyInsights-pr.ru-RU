---
title: Устранение неполадок в доступе, отказано в сообщениях
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704907"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="04768-102">Устранение неполадок в доступе, отказано в сообщениях</span><span class="sxs-lookup"><span data-stu-id="04768-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="04768-103">Если кто-то получил сообщение "Отказано в доступе" к общей папке в SharePoint, администратор коллекции сайтов мог включить режим блокировки разрешений пользователей с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="04768-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="04768-104">Чтобы отключить это:</span><span class="sxs-lookup"><span data-stu-id="04768-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="04768-105">Просмотрите сайт, щелкните значок Параметры, а затем нажмите **параметры сайта**.</span><span class="sxs-lookup"><span data-stu-id="04768-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="04768-106">В разделе **Администрирование семейства веб-сайтов** щелкните **Возможности семейства веб-сайтов**.</span><span class="sxs-lookup"><span data-stu-id="04768-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="04768-107">Рядом с **режимом блокировки разрешений** пользователей с ограниченным доступом щелкните **Deactivate**.</span><span class="sxs-lookup"><span data-stu-id="04768-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="04768-108">Сообщение об отказе в доступе может также возникать для общих папок, если сайт является сайтом публикации.</span><span class="sxs-lookup"><span data-stu-id="04768-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="04768-109">Сведения см. в [раздел Отказано в доступе при доступе к общей папке.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="04768-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="04768-110">Если кто-то получил сообщение "Отказано в доступе" при попытке просмотреть запросы на доступ, пользователь должен быть добавлен в качестве администратора коллекции сайтов или члена группы Владельцев для сайта.</span><span class="sxs-lookup"><span data-stu-id="04768-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="04768-111">Дополнительные сведения см. в списке "Отказ в доступе [к запросам доступа".](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="04768-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="04768-112">Если пользователь получил сообщение "Отказано в доступе" после удаления из локального каталога Active Directory и обратно, см. статью Access Denied, когда учетная запись пользователя синхронизирована с [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="04768-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

