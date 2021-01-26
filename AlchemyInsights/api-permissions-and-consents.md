---
title: Разрешения и согласие API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951921"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="0f76d-102">Разрешения и согласие API</span><span class="sxs-lookup"><span data-stu-id="0f76d-102">API permissions and consent</span></span>

<span data-ttu-id="0f76d-103">Приложения, которые интегрируются с платформой удостоверений Майкрософт, следуют модели авторизации, которая позволяет пользователям и администраторам управлять доступом к данным.</span><span class="sxs-lookup"><span data-stu-id="0f76d-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="0f76d-104">Реализация модели авторизации обновлена в конечной точке платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0f76d-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="0f76d-105">Он изменяет то, как приложение должно взаимодействовать с платформой удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0f76d-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="0f76d-106">[Разрешения и согласие в конечной](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) точке платформы удостоверений Майкрософт охватывают основные понятия этой модели авторизации, включая области, разрешения и согласие.</span><span class="sxs-lookup"><span data-stu-id="0f76d-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="0f76d-107">Платформа [согласия Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) упрощает разработку многоязычных веб-приложений и нативных клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="0f76d-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="0f76d-108">Эти приложения позволяют войти с помощью учетных записей пользователей из клиента Azure AD, который отличается от того, в котором зарегистрировано приложение.</span><span class="sxs-lookup"><span data-stu-id="0f76d-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="0f76d-109">Кроме того, им может потребоваться доступ к веб-API, таким как API Microsoft Graph (для доступа к Azure AD, Intune и службам в Microsoft 365) и другим API служб Майкрософт, а также к собственным веб-API.</span><span class="sxs-lookup"><span data-stu-id="0f76d-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

