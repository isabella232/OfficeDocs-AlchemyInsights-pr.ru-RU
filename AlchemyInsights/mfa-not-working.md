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
# <a name="issues-with-azure-mfa"></a>Проблемы с MFA Azure
Существует несколько вещей, которые необходимо проверить, не удается ли пользователям войти в систему с помощью многофакторной проверки подлинности (MFA)

1. Пострадавший пользователь может быть заблокирован на портале Azure Active Directory. В этом случае попытки проверки подлинности для этого конкретного пользователя будут автоматически отказано. [Выполните действия в этой статье, чтобы разблокировать их.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Если разблокирование пользователя не помогло или пользователь не заблокирован, вы можете попытаться сбросить MFA для пользователя, и они снова будут проходить процесс регистрации. [Следуйте шагам в этой статье.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Если это первый раз, когда вы включили MFA, и пользователи не могут войти в клиенты, не включив браузеры, такие как Outlook, Skype и т.д., возможно, ADAL (Библиотека проверки подлинности Active Directory) не включена в подписке на O365. В этом случае необходимо подключиться к Exchange Online Powershell и запустить этот кодлет:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled:$true*