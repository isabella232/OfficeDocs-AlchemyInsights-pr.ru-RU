---
title: Секрет клиента регистрации приложений или проблемы с сертификатами
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123199"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="e21ed-102">Секрет клиента регистрации приложений или проблемы с сертификатами</span><span class="sxs-lookup"><span data-stu-id="e21ed-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="e21ed-103">Истек срок действия секрета клиента приложения?</span><span class="sxs-lookup"><span data-stu-id="e21ed-103">Application client secret expiring?</span></span>

<span data-ttu-id="e21ed-104">Независимо от того, как было создано зарегистрированное приложение, будь то стандартный процесс регистрации на портале регистрации приложений или если директор службы был создан в клиенте с помощью согласия приложения, необходимо создать новый секрет клиента до истечения текущего и обновить в связанном коде приложения.</span><span class="sxs-lookup"><span data-stu-id="e21ed-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="e21ed-105">Максимальный срок действия — 2 года.</span><span class="sxs-lookup"><span data-stu-id="e21ed-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="e21ed-106">Напоминаем, что секретное значение должно быть записано, так как оно больше не будет видно после выхода со страницы регистрации приложений на портале.</span><span class="sxs-lookup"><span data-stu-id="e21ed-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="e21ed-107">Дополнительные сведения см. в [статью Quickstart: Регистрация](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) приложения на платформе удостоверений Майкрософт и лучшие практики [для платформы удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="e21ed-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="e21ed-108">Дополнительные данные см. в статью Создание приложения Azure AD & на [портале — платформа удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="e21ed-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
