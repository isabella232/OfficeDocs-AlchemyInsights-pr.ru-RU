---
title: Предоставление пользователям доступа к SharePoint и OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677220"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Предоставление пользователям доступа к SharePoint и OneDrive

> [!NOTE]
> Если сайт OneDrive или SharePoint недоступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная ошибка службы. [Проверка панели мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth)
  
Если вы хотите, чтобы сотрудники вашей организации могли входить в систему и использовать SharePoint и OneDrive, необходимо добавить учетные записи для них и убедиться, что у них есть лицензия, предоставляющая им доступ к SharePoint и OneDrive. Самый простой способ добавить пользователей в центре администрирования Microsoft 365.
  
1. Перейдите на [страницу активные пользователи в центре администрирования Microsoft 365](https://portal.office.com/adminportal/home#/users)и нажмите кнопку **Добавить пользователя**.
    
2. Введите сведения о пользователе и убедитесь, что в разделе **лицензии на продукты**назначена лицензия и выбрана **SharePoint Online** . 
    
Обратите внимание, что если вы разрешите внешний общий доступ в Организации, пользователи смогут делиться контентом SharePoint и OneDrive для пользователей за пределами Организации. Вам не нужно предоставлять лицензии на внешние пользователи. Кроме того, добавлять учетные записи для них не требуется, если только для общего доступа не задано значение "только существующие внешние пользователи". В этом случае, если пользователи не находятся в каталоге вашей организации, их необходимо добавить как гостей в центр администрирования Azure AD.
  

