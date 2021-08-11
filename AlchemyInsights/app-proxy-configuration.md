---
title: Конфигурация прокси-сервера приложения
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951578"
---
# <a name="app-proxy-configuration"></a>Конфигурация прокси-сервера приложения

1. Чтобы понять, как настроить прокси-приложение приложения в Azure AD, чтобы выставить локальное приложение в облако, см. в примере How [to configure an Application Proxy application.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Один вход (SSO) позволяет пользователям получать доступ к приложению без проверки подлинности несколько раз. Это позволяет единой проверке подлинности происходить в облаке, Azure Active Directory, и позволяет службе или соединителу выдать себя за пользователя, чтобы выполнить любые дополнительные проблемы проверки подлинности из приложения. Дополнительные дополнительные информации см. в статью Как настроить одно входное приложение [в приложении Прокси-приложения.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Используйте [эту статью](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) для устранения распространенных проблем, с которые сталкиваются люди при создании нового прокси-приложения приложения.
4. Если у вас возникли проблемы с настройкой back-end authentication в приложении, возможно, потребуется устранить проблемы с конфигурациями делегирования [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) для прокси-приложения или следовать указаниям по настройке приложения с [помощью PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) для решения проблемы.
