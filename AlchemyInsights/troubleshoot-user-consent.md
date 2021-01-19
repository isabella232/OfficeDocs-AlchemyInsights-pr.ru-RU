---
title: Устранение неполадок согласия пользователя
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897760"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="3cf60-102">Устранение неполадок согласия пользователя</span><span class="sxs-lookup"><span data-stu-id="3cf60-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="3cf60-103">Вы можете настроить, как конечные пользователи соглашаются с приложениями с помощью портала Azure или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3cf60-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="3cf60-104">Дополнительные [сведения см. в](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) параметрах согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="3cf60-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="3cf60-105">Администратор также может использовать [API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) для предоставления согласия на делегирование разрешений от имени одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3cf60-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="3cf60-106">Дополнительные сведения см. в сведениях о том, как получить доступ [от имени пользователя.](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="3cf60-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="3cf60-107">[Ошибки согласия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)пользователя : в этой статье обсуждаются ошибки, которые могут возникнуть в процессе согласия приложения.</span><span class="sxs-lookup"><span data-stu-id="3cf60-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="3cf60-108">Если вы устраняете непредвиденные запросы на согласие, не содержащие сообщений об ошибках, см. сценарии проверки подлинности [для Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="3cf60-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>