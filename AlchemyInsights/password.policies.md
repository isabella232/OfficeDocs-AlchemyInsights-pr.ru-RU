---
title: Политики паролей
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040843"
---
# <a name="password-policies"></a>Политики паролей

**У меня возникли проблемы с политикой паролей для пользователя**

- Политика паролей для пользователя зависит от того, является ли пользователь облачным или локально.
- Только пользователи облака должны выбрать пароль, отвечающий требованиям в этой статье: политики паролей, применимые только [к облачным учетным записям пользователей.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Локальному пользователю необходимо выбрать пароль, отвечающий требованиям локального доступа. Если локальному пользователю не удается установить пароль, проверьте свои требования к локальной сети.

**Я не знаю, как установить или проверить политики истечения срока действия пароля**

- Вы можете установить и проверить политику истечения срока действия для пользователей облака в клиенте с помощью PowerShell. Следуйте инструкциям в этой статье: Установите или проверьте политики паролей [с помощью PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Политика истечения срока действия пароля для локального пользователя задается в локальной AD.

**Другие полезные ссылки:**
- [Начало работы с сбросом пароля](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Устранение неполадок с инициированным администратором сбросом пароля](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
