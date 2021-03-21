---
title: Создание пользователя
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718198"
---
# <a name="create-user"></a><span data-ttu-id="7a910-102">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="7a910-102">Create user</span></span>

<span data-ttu-id="7a910-103">**ОБЪЯВЛЕНИЕ:**</span><span class="sxs-lookup"><span data-stu-id="7a910-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="7a910-104">[Обесценение поддержки регистрации WebView от Google с 4 января 2021 г.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="7a910-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="7a910-105">Проверьте, могут ли приложения оказаться затронутыми, следуя указаниям [Google](https://go.microsoft.com/fwlink/?linkid=2157323) по тестированию совместимости.</span><span class="sxs-lookup"><span data-stu-id="7a910-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="7a910-106">Убедитесь, что при входе в учетные записи Google пользователи используют веб-просмотр системы или системный браузер.</span><span class="sxs-lookup"><span data-stu-id="7a910-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="7a910-107">Дополнительные сведения см. в статье [Проблемы при входе в приложения с помощью браузера Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="7a910-107">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="7a910-108">**Не удается создать нового пользователя в каталоге Azure AD**</span><span class="sxs-lookup"><span data-stu-id="7a910-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="7a910-109">Убедитесь, что у вас есть разрешение на создание нового стандартного пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a910-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="7a910-110">Создать нового стандартного пользователя может только роль глобального администратора или администратора пользователя в Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="7a910-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="7a910-111">Если у вас нет одной из этих ролей, попросите администратора назначить вам одну из этих ролей или создать для вас новую учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a910-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="7a910-112">Убедитесь, что имя пользователя находится в домене, проверенном в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a910-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="7a910-113">Если в Azure AD нет проверенных имен личного домена, вы можете использовать исходный домен Azure AD, заканчивающийся на \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="7a910-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="7a910-114">Убедитесь, что имя пользователя находится в домене, который не включен в федерацию Azure AD из локальной среды Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7a910-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="7a910-115">Пользователи с доменными именами, включенными в федерацию из локальной среды, не могут быть добавлены в облако.</span><span class="sxs-lookup"><span data-stu-id="7a910-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="7a910-116">Убедитесь, что другие пользователи или контакты не используют имя, которое необходимо назначить новому пользователю.</span><span class="sxs-lookup"><span data-stu-id="7a910-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="7a910-117">Имена пользователей в Azure AD должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="7a910-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="7a910-118">См. [роли и администраторы Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для вашей службы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a910-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="7a910-119">См. [имена доменов](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для вашей службы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a910-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="7a910-120">Чтобы получить подробные сведения о недавно созданном или удаленном пользователе, например о том, кто и когда выполнил это действие, проверьте [журналы аудита](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators).</span><span class="sxs-lookup"><span data-stu-id="7a910-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="7a910-121">Дополнительные сведения о добавлении новых пользователей см. в сайте Использование портала Azure для создания нового пользователя [в Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="7a910-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="7a910-122">[Административные роли Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)разрешения на роль администратора в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7a910-122">[Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="7a910-123">Вы также можете [использовать Azure AD PowerShell для создания нового пользователя.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="7a910-123">You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>