---
title: Процесс разрешений и согласия API
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379894"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="71c66-102">Процесс разрешений и согласия API</span><span class="sxs-lookup"><span data-stu-id="71c66-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="71c66-103">Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия.</span><span class="sxs-lookup"><span data-stu-id="71c66-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="71c66-104">[В справке разрешений Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) перечислены разрешения, связанные с каждым основным набором API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71c66-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="71c66-105">В ней также приведены руководства по использованию разрешений.</span><span class="sxs-lookup"><span data-stu-id="71c66-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="71c66-106">**Настройка или обновление основного**</span><span class="sxs-lookup"><span data-stu-id="71c66-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="71c66-107">[Создание serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) . В этой статье показано, как создать новый объект servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="71c66-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="71c66-108">Создание на портале & приложения Azure [AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) — в этой статье показано, как создать новое приложение Azure Active Directory (Azure AD), которое можно использовать с помощью управления доступом на основе ролей.</span><span class="sxs-lookup"><span data-stu-id="71c66-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="71c66-109">[Принципы & службы в Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) . В этой статье описываются регистрация приложений, объекты приложений и принципы службы в Azure Active Directory: что они, как они используются и как они связаны друг с другом.</span><span class="sxs-lookup"><span data-stu-id="71c66-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="71c66-110">**Добавление или обновление регистрации приложений и предоставление согласия администратора**</span><span class="sxs-lookup"><span data-stu-id="71c66-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="71c66-111">[Создание регистрации приложения](https://docs.microsoft.com/graph/api/application-post-applications) . В этой статье показано, как создать новый объект приложения.</span><span class="sxs-lookup"><span data-stu-id="71c66-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="71c66-112">[Обновление регистрации приложения - разрешения API](https://docs.microsoft.com/graph/api/application-update) . В этой статье показано, как обновить свойства объекта приложения.</span><span class="sxs-lookup"><span data-stu-id="71c66-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="71c66-113">[Предоставление согласия администратора](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) . Для согласия администратора и согласия в целом, мы требуем, чтобы администратор явно дает согласие.</span><span class="sxs-lookup"><span data-stu-id="71c66-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="71c66-114">[RBAC (бета-версия)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) — контейнер управления ролью для унифицированных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, которые поддерживают несколько принципов и несколько областей в одном назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="71c66-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="71c66-115">Это отличается от типа ресурса *rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="71c66-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="71c66-116">Microsoft Intune является примером такого поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="71c66-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="71c66-117">Назначение ролей в Intune может иметь массив принципалов и массив групп областей.</span><span class="sxs-lookup"><span data-stu-id="71c66-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="71c66-118">**Это бета-версия, что означает, что она еще находится в разработке и не рекомендуется для использования в производстве.**</span><span class="sxs-lookup"><span data-stu-id="71c66-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
