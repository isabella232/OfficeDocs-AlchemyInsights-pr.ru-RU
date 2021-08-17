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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084359"
---
# <a name="sso-connection-issues"></a>Проблемы подключения к SSO

1. Следуйте инструкциям, приведенным в статье [Краткое руководство: Настройка свойств приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure), чтобы настроить приложение.
2. В зависимости от [](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) выбранного приложения и выбранного параметра единой регистрации следуйте соответствующим указаниям:
    - Чтобы настроить  локальное приложение для единого входного приложения на основе **SAML,** см. в примере [SAML single-sign-on для](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)локального приложения с помощью прокси-приложения.
    - Чтобы настроить **облачное приложение для** единой входной записи на основе **пароля,** см. в приложении [Configure password single sign-on.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Чтобы настроить  локальное приложение для единой входной записи через **прокси-сервер** приложения, см. в примере Сводка паролей для единой входной записи [с помощью прокси-сервера приложения.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Устранение** неполадок с прокси-серверами приложений: рекомендуется начать [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)с проверки потока устранения неполадок, устранения проблем соединителю прокси-сервера приложений, чтобы определить, правильно ли настроены соединители прокси-серверов приложений. Если у вас по-прежнему возникли проблемы с подключением к приложению, следуйте потоку устранения [неполадок](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)в проблемах приложения-прокси-сервера отладки приложений. Вы можете [идентифицировать проблемы CORS с](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) помощью средств отлаговки браузера:
    - Запустите браузер и перейдите в веб-приложение.
    - Нажмите клавишу **F12**, чтобы вывести консоль отладки.
    - Попробуйте воспроизвести транзакцию и просмотрите сообщение консоли. Нарушение CORS вызывает консольную ошибку о происхождении.
    - Некоторые проблемы CORS не могут быть решены, например, когда приложение перенаправляет login.microsoft.com проверку подлинности, а срок действия маркера доступа истекает. После этого вызов CORS не удается. Временное решение для этого сценария — продлить жизненный цикл маркера доступа, чтобы предотвратить истечение его срока действия в течении сеанса пользователя. Дополнительные сведения о том, как это сделать, см. в статье [Настраиваемые жизненные циклы маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Устранение неполадок на основе единого входного номера на основе **SAML:** мы рекомендуем проверить проблемы, связанные с входом в настроенные приложения на основе единого входного знака на основе [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)чтобы найти решения проблем, с которыми вы, скорее всего, столкнетесь.
5. **Устранение** неполадок с одним входом на основе пароля: мы рекомендуем проверить устранение неполадок, основанных на одном входе на основе пароля в [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)чтобы найти решения проблем, с которыми вы, скорее всего, столкнетесь.
6. О проблемах с подключением при использовании VPN см. в документе How [to use single sign on (SSO) над VPN и Wi-Fi подключениями.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
