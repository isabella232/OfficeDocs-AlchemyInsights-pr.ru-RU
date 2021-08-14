---
title: Проблемы владельца регистрации приложений
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951146"
---
# <a name="app-registration-owner-issues"></a>Проблемы владельца регистрации приложений

Ниже 1. Доступные методы добавления принципов в качестве владельцев для регистрации приложений:

- Использование модуля PowerShell Azure AD —

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Справка: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Использование CLI Azure — `az ad app owner add`

    Справка: [владелец приложения az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Использование ms Graph -

    Справка: [Добавление владельца - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Использование портала Azure AD — перейдите portal.azure.com [>](https://portal.azure.com/) Azure Active directory > регистрация приложений > Выберите приложение > Владельцы > Добавить владельцев

**Не удается просмотреть приложение на лезвии Регистрации приложений, даже если вы владелец этого приложения?**

Владелец приложения не является административной ролью. Если включен параметр Ограничение доступа к порталу администрирования [Azure AD,](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) только администратор сможет просматривать приложения на портале регистрации приложений. Чтобы владелец мог просматривать приложения, либо отключите этот параметр (установите значение НЕТ), либо назначьте ему роль администратора только для конкретного приложения. Однако для этого потребуется лицензия Azure AD Premium P2 и включить [управление привилегированными пользователями](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
