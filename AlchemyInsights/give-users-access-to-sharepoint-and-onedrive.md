---
title: Предоставление пользователям доступа к SharePoint и OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36523776"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="72092-102">Предоставление пользователям доступа к SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="72092-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="72092-103">Если сайт OneDrive или SharePoint недоступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная ошибка службы.</span><span class="sxs-lookup"><span data-stu-id="72092-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="72092-104">Проверка панели мониторинга работоспособности службы</span><span class="sxs-lookup"><span data-stu-id="72092-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="72092-105">Если вы хотите, чтобы сотрудники вашей организации могли входить в систему и использовать SharePoint и OneDrive, необходимо добавить учетные записи для них и убедиться, что у них есть лицензия, предоставляющая им доступ к SharePoint и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="72092-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="72092-106">Самый простой способ добавить пользователей в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="72092-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="72092-107">Перейдите на [страницу активные пользователи в центре администрирования Microsoft 365](https://portal.office.com/adminportal/home#/users)и нажмите кнопку **Добавить пользователя**.</span><span class="sxs-lookup"><span data-stu-id="72092-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="72092-108">Введите сведения о пользователе и убедитесь, что в разделе **лицензии на продукты**назначена лицензия и выбрана **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="72092-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="72092-109">Обратите внимание, что если вы разрешите внешний общий доступ в Организации, пользователи смогут делиться контентом SharePoint и OneDrive для пользователей за пределами Организации.</span><span class="sxs-lookup"><span data-stu-id="72092-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="72092-110">Вам не нужно предоставлять лицензии на внешние пользователи.</span><span class="sxs-lookup"><span data-stu-id="72092-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="72092-111">Кроме того, добавлять учетные записи для них не требуется, если только для общего доступа не задано значение "только существующие внешние пользователи".</span><span class="sxs-lookup"><span data-stu-id="72092-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="72092-112">В этом случае, если пользователи не находятся в каталоге вашей организации, их необходимо добавить как гостей в центр администрирования Azure AD.</span><span class="sxs-lookup"><span data-stu-id="72092-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

