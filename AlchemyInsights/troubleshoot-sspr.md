---
title: Устранение неполадок SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038971"
---
# <a name="troubleshoot-sspr"></a>Устранение неполадок SSPR

**У меня возникли проблемы с настройкой сброса пароля**

- Если вы администратор и ищете, как включить сброс пароля самообслуживаемых, см. в учебнике включить [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), чтобы настроить сброс пароля для вашей организации. Кроме того, может потребоваться просмотреть [требования к лицензированию.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) В организации должна быть назначена по крайней мере одна лицензия.
    - **Только пользователи облака** — Office 365 (O365) платные SKU или Azure AD Basic
    - **Облачные и/или** локально пользователи — Azure AD Premium P1 или P2, Enterprise Mobility + Security (EMS) или Secure Productive Enterprise (SPE)
- Дополнительные вопросы об сбросе паролей самообслуживаем читайте [в нашем faQ.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Я получаю сообщение об ошибке**

Просмотрите эту статью, чтобы найти распространенные ошибки и их решения: сброс пароля [самообслуживления](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**У меня возникли проблемы с политикой сброса паролей**

- Если политика сброса паролей ведет себя не так, как ожидалось, или у вас возникли вопросы по политикам сброса [паролей,](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)просмотрите эту статью: политики паролей и ограничения в Azure Active Directory .
- Политики сброса паролей не применяются к администраторам. Корпорация Майкрософт применяет сильную политику сброса паролей с двумя воротами по умолчанию для любой роли администратора Azure. Убедитесь, что вы тестируете с пользователем, который не является администратором. Дополнительные сведения о политике сброса администратора см. в этой [статье.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Я не хочу, чтобы мои пользователи регистрируют дополнительные сведения о безопасности для сброса пароля**

Вы можете предварительно заполнить данные (атрибуты электронной почты и телефона) для пользователей с помощью API, PowerShell или Azure AD Подключение. Чтобы узнать, как читать:

- [Развертывание сброса пароля без необходимости регистрации пользователей](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Какие данные используются при сбросе пароля](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Я хочу, чтобы мои пользователи зарегистрировали свои дополнительные сведения о безопасности для сброса пароля**

1. Чтобы пользователи зарегистрировали свои сведения о безопасности для сброса пароля самообслуживки, направив их на [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. После заполнения данных пользователем (пользователем или администратором) направите aka.ms/sspr, чтобы пользователи могли сбросить собственные пароли. [](https://passwordreset.microsoftonline.com/)
1. Если пользователи по-прежнему испытывают проблемы, они, скорее всего, **федерария** или **пароль hash synched** пользователей. Это означает, что существует проблема со службой записи паролей.