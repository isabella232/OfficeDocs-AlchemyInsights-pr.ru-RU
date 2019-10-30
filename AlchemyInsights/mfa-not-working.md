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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768850"
---
# <a name="issues-with-azure-mfa"></a>Проблемы с Azure MFA
Существует несколько моментов, которые необходимо проверить, не могут ли пользователи входить в систему с помощью многофакторной проверки подлинности (MFA)

1. Затронутого пользователя можно заблокировать на портале Azure Active Directory. В этом случае попытки проверки подлинности для определенного пользователя будут автоматически отклонены. [Выполните действия, описанные в этой статье, чтобы разблокировать их.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Если разблокирование пользователя не помогает или пользователь не заблокирован, вы можете попытаться сбросить MFA для пользователя и снова пройти процесс регистрации. [Выполните действия, описанные в этой статье.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Если вы впервые включили MFA, и ваши пользователи не могут выполнять вход в клиенты, не поддерживающие браузеры, такие как Outlook, Skype и т. д., например, ADAL (Библиотека проверки подлинности Active Directory) не включена в вашей подписке на Office 365. В этом случае вам потребуется подключиться к Exchange Online PowerShell и выполнить следующий командлет:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*