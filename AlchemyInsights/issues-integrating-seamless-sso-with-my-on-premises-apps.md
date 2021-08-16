---
title: Проблемы с интеграцией бесшовных SSO с локальной программой
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028305"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Проблемы с интеграцией бесшовных SSO с локальной программой

Чтобы устранить проблемы с интеграцией бесшовных SSO с локальной приложениями, сделайте следующее:

**Рекомендуемые действия**

1. Чтобы настроить  локальное приложение для единой входной записи через **прокси-сервер** приложения, см. в примере Сводка паролей для единой входной записи [с помощью прокси-сервера приложения.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Устранение** неполадок с прокси-серверами приложений. Рекомендуется начать [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)с проверки потока устранения неполадок, устранения проблем соединителю прокси-сервера приложений, чтобы определить, правильно ли настроены соединители прокси-серверов приложений. Если у вас по-прежнему возникают проблемы с подключением к приложению, выполните действия по устранению неполадок в статье [Отладка проблем с прокси приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Проблемы с [CORS можно определить](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) с помощью следующих средств отлаговки браузера:
    1. Запустите браузер и перейдите в веб-приложение.
    1. Нажмите клавишу **F12**, чтобы вывести консоль отладки.
    1. Попробуйте воспроизвести транзакцию и просмотрите сообщение консоли. Нарушение CORS вызывает консольную ошибку о происхождении.
    1. Некоторые проблемы CORS не могут быть устранены, например, когда приложение перенаправляет login.microsoftonline.com проверку подлинности, а срок действия маркера доступа истекает. После этого вызов CORS не удается. Временное решение для этого сценария — продлить жизненный цикл маркера доступа, чтобы предотвратить истечение его срока действия в течении сеанса пользователя. Дополнительные сведения о том, как это сделать, см. в статье [Настраиваемые жизненные циклы маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Рекомендуемые документы**

- [Настройка единого входного знака в приложении Прокси-приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Единое входное приложение SAML для локального приложения с прокси-сервером приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Понимание и решение Azure Active Directory прокси-серверов приложений](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Устранение неполадок с настойками ограниченного делегирования Kerberos для прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)