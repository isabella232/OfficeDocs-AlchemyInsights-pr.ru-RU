---
title: Предоставление пользователям доступа к SharePoint и OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 5a1cdeefa4474e8ce0e6a7a37be016cc87b9791d
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308380"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="e9dfb-102">Предоставление пользователям доступа к SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="e9dfb-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="e9dfb-p101">Если сайт SharePoint или OneDrive к нескольким пользователям, которые ранее имели доступ недоступен, может быть проблема временной службы. [Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="e9dfb-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="e9dfb-p102">Если необходимо предоставить пользователям в вашей организации должны иметь возможность выполнять вход и использовать SharePoint и OneDrive, необходимо добавить учетные записи для их и убедитесь, что у них есть лицензии, который предоставляет доступ к SharePoint и OneDrive. В центре администрирования Office 365 — это самый простой способ добавления пользователей.</span><span class="sxs-lookup"><span data-stu-id="e9dfb-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="e9dfb-107">Перейдите на [страницу активных пользователей в центре администрирования Office 365](https://portal.office.com/adminportal/home#/users)и нажмите кнопку **Добавить пользователя**.</span><span class="sxs-lookup"><span data-stu-id="e9dfb-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="e9dfb-108">Введите данные для пользователя и убедитесь в том, что в разделе **лицензий на продукт**, лицензия назначена и установлен **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="e9dfb-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="e9dfb-p103">Обратите внимание, что если разрешить внешние общего доступа в организации, пользователи могут совместно использовать содержимого SharePoint и OneDrive с людьми за пределами организации. Передайте эти лицензии внешним пользователям не нужно. Также не требуется для добавления учетных записей для их, если общий доступ к не задано значение «Только существующие внешние пользователи.» В этом случае люди в телефонном справочнике организации, требуется ли добавить их в качестве гостя пользователей в центре администрирования Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9dfb-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

