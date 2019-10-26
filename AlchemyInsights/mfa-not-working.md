---
title: Проблемы с MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545191"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="b4e06-102">Проблемы с MFA</span><span class="sxs-lookup"><span data-stu-id="b4e06-102">Issues with MFA</span></span>
<span data-ttu-id="b4e06-103">Существует несколько моментов, которые необходимо проверить, не может ли пользователь войти с использованием многофакторной проверки подлинности (MFA)</span><span class="sxs-lookup"><span data-stu-id="b4e06-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b4e06-104">Затронутого пользователя можно заблокировать на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4e06-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b4e06-105">В этом случае попытки проверки подлинности для определенного пользователя будут автоматически отклонены.</span><span class="sxs-lookup"><span data-stu-id="b4e06-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b4e06-106">Выполните действия, описанные в этой статье, чтобы разблокировать их.</span><span class="sxs-lookup"><span data-stu-id="b4e06-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b4e06-107">Если разблокирование пользователя не помогает или пользователь не заблокирован, вы можете попытаться сбросить MFA для пользователя и снова пройти процесс регистрации.</span><span class="sxs-lookup"><span data-stu-id="b4e06-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b4e06-108">Выполните действия, описанные в этой статье.</span><span class="sxs-lookup"><span data-stu-id="b4e06-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b4e06-109">Если вы впервые включили MFA, и ваши пользователи не могут выполнять вход в клиенты, не поддерживающие браузеры, такие как Outlook, Skype и т. д., например, ADAL (Библиотека проверки подлинности Active Directory) не включена в вашей подписке на Office 365.</span><span class="sxs-lookup"><span data-stu-id="b4e06-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b4e06-110">В этом случае вам потребуется подключиться к Exchange Online PowerShell и выполнить следующий командлет:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="b4e06-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>