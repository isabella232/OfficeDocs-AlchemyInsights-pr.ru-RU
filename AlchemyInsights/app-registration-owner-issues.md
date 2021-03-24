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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123196"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="80a31-102">Проблемы владельца регистрации приложений</span><span class="sxs-lookup"><span data-stu-id="80a31-102">App Registration Owner issues</span></span>

<span data-ttu-id="80a31-103">Ниже 1. Доступные методы добавления принципов в качестве владельцев для регистрации приложений:</span><span class="sxs-lookup"><span data-stu-id="80a31-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="80a31-104">Использование модуля PowerShell Azure AD —</span><span class="sxs-lookup"><span data-stu-id="80a31-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="80a31-105">Справка: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="80a31-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="80a31-106">Использование CLI Azure — `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="80a31-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="80a31-107">Справка: [владелец приложения az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="80a31-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="80a31-108">Использование MS Graph —</span><span class="sxs-lookup"><span data-stu-id="80a31-108">Using MS Graph -</span></span>

    <span data-ttu-id="80a31-109">Справка: [Добавление владельца - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="80a31-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="80a31-110">Использование портала Azure AD — перейдите portal.azure.com [>](https://portal.azure.com/) Azure Active directory > регистрация приложений > Выберите приложение > Владельцы > Добавить владельцев</span><span class="sxs-lookup"><span data-stu-id="80a31-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="80a31-111">**Не удается просмотреть приложение на лезвии Регистрации приложений, даже если вы владелец этого приложения?**</span><span class="sxs-lookup"><span data-stu-id="80a31-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="80a31-112">Владелец приложения не является административной ролью.</span><span class="sxs-lookup"><span data-stu-id="80a31-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="80a31-113">Если включен параметр Ограничение доступа к порталу администрирования [Azure AD,](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) только администратор сможет просматривать приложения на портале регистрации приложений.</span><span class="sxs-lookup"><span data-stu-id="80a31-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="80a31-114">Чтобы владелец мог просматривать приложения, либо отключите этот параметр (установите значение НЕТ), либо назначьте ему роль администратора только для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="80a31-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="80a31-115">Однако для этого потребуется лицензия Azure AD Premium P2 и включить управление [привилегированными удостоверениями.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="80a31-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
