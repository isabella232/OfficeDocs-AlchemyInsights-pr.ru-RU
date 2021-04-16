---
title: Проблемы с MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810497"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="97b3c-102">Проблемы с MFA Azure</span><span class="sxs-lookup"><span data-stu-id="97b3c-102">Issues with Azure MFA</span></span>
<span data-ttu-id="97b3c-103">Существует несколько вещей, которые необходимо проверить, не удается ли пользователям войти в систему с помощью многофакторной проверки подлинности (MFA)</span><span class="sxs-lookup"><span data-stu-id="97b3c-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="97b3c-104">Пострадавший пользователь может быть заблокирован на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="97b3c-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="97b3c-105">В этом случае попытки проверки подлинности для этого конкретного пользователя будут автоматически отказано.</span><span class="sxs-lookup"><span data-stu-id="97b3c-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="97b3c-106">Выполните действия в этой статье, чтобы разблокировать их.</span><span class="sxs-lookup"><span data-stu-id="97b3c-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="97b3c-107">Если разблокирование пользователя не помогло или пользователь не заблокирован, вы можете попытаться сбросить MFA для пользователя, и они снова будут проходить процесс регистрации.</span><span class="sxs-lookup"><span data-stu-id="97b3c-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="97b3c-108">Следуйте шагам в этой статье.</span><span class="sxs-lookup"><span data-stu-id="97b3c-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="97b3c-109">Если это первый раз, когда вы включили MFA, и пользователи не могут войти в клиенты, не включив браузеры, такие как Outlook, Skype и т.д., возможно, ADAL (Библиотека проверки подлинности Active Directory) не включена в подписке на O365.</span><span class="sxs-lookup"><span data-stu-id="97b3c-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="97b3c-110">В этом случае необходимо подключиться к Exchange Online Powershell и запустить этот кодлет:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="97b3c-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>