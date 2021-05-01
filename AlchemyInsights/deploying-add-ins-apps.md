---
title: Развертывание надстройок для Приложения Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107532"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Развертывание надстройок для Приложения Microsoft 365

Централизованное развертывание — это рекомендуемый способ развертывания надстройок Office пользователям и группам в вашей организации. Чтобы развернуть надстройки, выполните следующие действия:

**Примечание:** Чтобы установить надстройки для Office как отдельного пользователя, см. просмотр, управление и установка надстройок в [Office программах.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Кроме того, убедитесь, что включено индивидуальное приобретение надстройок Office Store. 

1. Убедитесь, что среда соответствует требованиям для развертывания надстройок с помощью централизованного развертывания. Подробные сведения см. [в материале Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Перейдите **Параметры** Интегрированные приложения Получить приложения в центре администрирования Microsoft 365 для развертывания  >    >   надстройок. 

Примечания. 

- Интегрированные приложения требуют, чтобы у администратора были разрешения глобального администратора или Exchange администратора.

- При развертывании надстройок для нескольких пользователей рекомендуется выполнять назначения с помощью групп, а не отдельных пользователей. Дополнительные сведения [см. в материале Considerations when assigning an add-in to users and groups.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Централизованное развертывание не поддерживает пользователей в вложенных группах или группах с родительскими группами. Подробные сведения см. [в материале User and group assignments.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Убедитесь Microsoft 365 что служба управления приложениями (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a' включена для входа пользователей. Подробные сведения см. [в материале Настройка свойств приложений.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Если вы испытываете проблемы с развертыванием надстройок с помощью интегрированных приложений, попробуйте развернуть их с помощью [надстройки.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Дополнительные сведения:

[Развертывание надстройок в центре администрирования](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Управление надстройкими в центре администрирования](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 Чтобы управлять надстройкими, используйте централизованные [комлеты Deployment PowerShell](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Публикация Office надстройки](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) с помощью центраализованного развертывания Microsoft 365 центра администрирования 
 [Устранение неполадок. Пользователь не видит надстройки](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Устранение ошибок пользователей с Office надстройки](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)