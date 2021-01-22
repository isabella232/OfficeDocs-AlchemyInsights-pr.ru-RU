---
title: Проблемы подключения к SSO
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
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918147"
---
# <a name="sso-connection-issues"></a>Проблемы подключения к SSO

1. Следуйте инструкциям, приведенным в статье [Краткое руководство: Настройка свойств приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure), чтобы настроить приложение.
2. В зависимости от выбранного [приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) и варианта единого входов следуйте соответствующим рекомендациям ниже:
    - Чтобы настроить  локальное приложение для единого входов на основе **SAML,** см. статью "Единый вход SAML для локального приложения с прокси-сервером [приложения".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Чтобы настроить облачное **приложение** для единого входов на основе паролей, см. ["Настройка единого пароля".](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Чтобы настроить  локальное приложение для единого доступа через **прокси-сервер** приложения, см. статью "Хранилище паролей для единого доступа с помощью прокси [приложения".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. Устранение неполадок прокси **приложения:** рекомендуем начать с проверки потока устранения неполадок, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)отладки соединителю прокси приложения, чтобы определить, правильно ли настроены соединители прокси приложения. Если у вас по-прежнему возникли проблемы с подключением к приложению, следуйте потоку устранения неполадок в области ["Отладка](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)проблем с прокси-сервером приложения". Проблемы [CORS можно определить с](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) помощью средств отлаки браузера:
    - Запустите браузер и перейдите в веб-приложение.
    - Нажмите клавишу **F12**, чтобы вывести консоль отладки.
    - Попробуйте воспроизвести транзакцию и просмотрите сообщение консоли. Нарушение CORS вызывает консольную ошибку о происхождении.
    - Некоторые проблемы CORS не могут быть решены, например, когда приложение перенаправляется на login.microsoft.com для проверки подлинности и срок действия маркера доступа истекает. Вызов CORS затем не удается. Временное решение для этого сценария — продлить жизненный цикл маркера доступа, чтобы предотвратить истечение его срока действия в течении сеанса пользователя. Дополнительные сведения о том, как это сделать, см. в статье [Настраиваемые жизненные циклы маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Устранение неполадок с единым входом на основе **SAML:** мы рекомендуем проверить проблемы, связанные с входом в настроенные приложения с единым входом на основе [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)чтобы найти решения проблем, с которыми вы чаще всего сталкиваетесь.
5. **Устранение** неполадок единого доступа на основе паролей: мы рекомендуем проверить устранение неполадок единого доступа на основе паролей в [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)чтобы найти решения проблем, с которыми вы чаще всего сталкиваетесь.
6. О проблемах с подключением при использовании VPN см. в документе "Использование единого входного подключения [(SSO) по VPN и Wi-Fi подключениям".](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
