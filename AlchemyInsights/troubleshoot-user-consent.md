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
# <a name="troubleshoot-user-consent"></a>Устранение неполадок согласия пользователя

1. Вы можете настроить, как конечные пользователи соглашаются с приложениями с помощью портала Azure или PowerShell. Дополнительные [сведения см. в](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) параметрах согласия пользователя.
1. Администратор также может использовать [API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) для предоставления согласия на делегирование разрешений от имени одного пользователя. Дополнительные сведения см. в сведениях о том, как получить доступ [от имени пользователя.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Ошибки согласия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)пользователя : в этой статье обсуждаются ошибки, которые могут возникнуть в процессе согласия приложения. Если вы устраняете непредвиденные запросы на согласие, не содержащие сообщений об ошибках, см. сценарии проверки подлинности [для Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)