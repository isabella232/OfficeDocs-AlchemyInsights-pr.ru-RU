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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007911"
---
# <a name="troubleshoot-user-consent"></a>Устранение неполадок согласия пользователя

1. Вы можете настроить согласие конечных пользователей на приложения через портал Azure или PowerShell. Дополнительные [сведения см. в параметрах](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) согласия пользователя.
1. Администратор также может использовать [API microsoft Graph для](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) предоставления согласия на делегирование разрешений от имени одного пользователя. Дополнительные сведения [см. в статью Получить](https://docs.microsoft.com/graph/auth-v2-user)доступ от имени пользователя.
1. [Ошибки согласия пользователя:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)в этой статье обсуждаются ошибки, которые могут возникать в процессе согласия на приложение. Если вы устраняете непредвиденные запросы согласия, не содержащие сообщений об ошибках, см. в тексте Сценарии проверки подлинности [для Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)