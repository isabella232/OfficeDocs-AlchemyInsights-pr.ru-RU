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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123199"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Секрет клиента регистрации приложений или проблемы с сертификатами

Истек срок действия секрета клиента приложения?

Независимо от того, как было создано зарегистрированное приложение, будь то стандартный процесс регистрации на портале регистрации приложений или если директор службы был создан в клиенте с помощью согласия приложения, необходимо создать новый секрет клиента до истечения текущего и обновить в связанном коде приложения. Максимальный срок действия — 2 года. Напоминаем, что секретное значение должно быть записано, так как оно больше не будет видно после выхода со страницы регистрации приложений на портале. Дополнительные сведения см. в [статью Quickstart: Регистрация](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) приложения на платформе удостоверений Майкрософт и лучшие практики [для платформы удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Дополнительные данные см. в статью Создание приложения Azure AD & на [портале — платформа удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
