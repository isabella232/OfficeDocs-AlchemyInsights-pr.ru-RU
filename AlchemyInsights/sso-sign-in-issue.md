---
title: Проблемы с беспроблимным входом пользователей в SSO
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919209"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Проблемы с беспроблимным входом пользователей в SSO

После проверки подлинности пользователя браузер будет кэшировать учетные данные пользователя, чтобы в том же браузере приложение автоматически включит в себя ту же учетную запись. Это может затруднить для другого пользователя или одного пользователя вход в несколько учетных записей на одном устройстве. Чтобы решить эту проблему: 1. Попробуйте вход в другой браузер. 2. Очистка кэша браузера и/или файлов cookie и повторная попытка входить в него.

Если у вас по-прежнему возникли проблемы со входом, рекомендуем следующее для диагностики и автоматизации действий по разрешению:

1. Установите расширение [безопасного](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) браузера "Мои приложения", чтобы помочь Azure Active Directory (Azure AD) улучшить диагностику и разрешение при использовании тестирования на портале Azure.
2. Воспроизведет ошибку с помощью тестирования на странице конфигурации приложения на портале Azure. Дополнительные см. в документе ["Отламывка](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)приложений единого входов на основе SAML".
3. Если вы используете тестирование на портале Azure с расширением безопасного браузера "Мои приложения", вы можете **пропустить шаг 4.**
4. Чтобы открыть страницу конфигурации единого входов samL, спишитесь:
    - Откройте портал [Azure и](https://portal.azure.com/) во sign in as a **Global Administrator** or **Coadmin**.
    - Откройте расширение **Azure Active Directory,** выбрав все службы в верхней части основного левого меню навигации. 
    - Введите "Azure Active Directory" в поле поиска фильтра и выберите элемент **Azure Active Directory.**
    - Выберите **"Корпоративные приложения" в** левом меню навигации Azure Active Directory.
    - Выберите **"Все приложения",** чтобы просмотреть список всех приложений. Если вы не видите нужное приложение, используйте  этот параметр в  верхней части списка "Все приложения" и установите для параметра **"Показать"** параметр "Все **приложения".**
    - Выберите приложение, которое необходимо настроить для единого входов.
    - После загрузки приложения  выберите "Единый вход" в левом меню навигации приложения.
    - Выберите **SSO на основе SAML.**
5. В зависимости от ошибки, чтобы узнать больше о рекомендуемых действиях, см. проблемы при входе в настроенные приложения с единым входом на основе [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Чтобы устранить другие проблемы со входом пользователя, обратитесь к следующему руководству:
    - [Протокол Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [How to: Troubleshoot sign-in errors using Azure Active Directory reports](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Непредвиденное запрос на согласие](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Ошибка согласия пользователя](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Проблемы при входе из my Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Ошибка на странице "Вход в приложение"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Проблема при входе в приложение Microsoft App](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
