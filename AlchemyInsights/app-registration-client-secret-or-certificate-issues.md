---
title: Секрет клиента регистрации приложений или проблемы с сертификатами
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951506"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Секрет клиента регистрации приложений или проблемы с сертификатами

Истек срок действия секрета клиента приложения?

Независимо от того, как было создано зарегистрированное приложение, будь то стандартный процесс регистрации на портале регистрации приложений или если директор службы был создан в клиенте с помощью согласия приложения, необходимо создать новый секрет клиента до истечения текущего и обновить в связанном коде приложения. Максимальный срок действия — 2 года. Напоминаем, что секретное значение должно быть записано, так как оно больше не будет видно после выхода со страницы регистрации приложений на портале. Дополнительные сведения см. в [статью Quickstart: Регистрация](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) приложения в платформа удостоверений Майкрософт и лучшие практики для [платформа удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Дополнительные дополнительные возможности см. в статью Создание приложения Azure AD & на [портале — платформа удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
