---
title: Проблемы с согласием администратора
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888322"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="e4245-102">Проблемы с согласием администратора</span><span class="sxs-lookup"><span data-stu-id="e4245-102">Admin consent issues</span></span>

1. <span data-ttu-id="e4245-103">Разрешить рабочий [процесс согласия администратора,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) чтобы пользователи могли запрашивать утверждение администратора непосредственно с экрана согласия.</span><span class="sxs-lookup"><span data-stu-id="e4245-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="e4245-104">Если во время получения согласия вы или пользователи приложения видите непредвиденные ошибки, см. эту статью для устранения неполадок: непредвиденное сообщение об ошибке при выполнении согласия [на приложение.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="e4245-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="e4245-105">Узнайте больше о согласии администратора на [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) платформе удостоверений [Майкрософт,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)о работе запроса согласия и о том, как оценить запрос согласия администратора на весь [клиент.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="e4245-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="e4245-106">Приложения, которые интегрируются с платформой удостоверений Майкрософт, следуют модели авторизации, которая позволяет пользователям и администраторам управлять доступом к данным.</span><span class="sxs-lookup"><span data-stu-id="e4245-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="e4245-107">Реализация модели авторизации была обновлена в конечной точке платформы удостоверений Майкрософт, и она изменяет то, как приложение должно взаимодействовать с платформой удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e4245-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="e4245-108">Обзор [этой модели](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) авторизации, включая области, разрешения и согласие, см. в сведениях о разрешениях и согласиях в конечной точке платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e4245-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>