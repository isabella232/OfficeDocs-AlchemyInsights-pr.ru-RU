---
title: Проблемы с интеграцией простого единого единого выпуска с моими приложениями
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848780"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Проблемы с интеграцией простого единого единого выпуска с моими приложениями

Для устранения неполадок интеграции простого единого и локального приложений сделайте следующее:

**Рекомендуемые действия**

1. Чтобы настроить  локальное приложение для единого доступа через **прокси-сервер** приложения, см. статью "Хранилище паролей для единого доступа с помощью прокси [приложения".](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. Устранение неполадок прокси **приложения:** рекомендуем начать с проверки потока устранения неполадок, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)отладки соединителю прокси приложения, чтобы определить, правильно ли настроены соединители прокси приложения. Если у вас по-прежнему возникли проблемы с подключением к приложению, выполните действия по устранению неполадок, которые необходимо предпринять при устранении неполадок, имеющихся в приложении ["Отладка](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)прокси приложения". Проблемы [CORS можно определить с](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) помощью следующих средств отлаки браузера:
    1. Запустите браузер и перейдите к веб-приложению.
    1. Нажмите **F12,** чтобы вывести консоль отлаки.
    1. Попробуйте воспроизвести транзакцию и просмотрите сообщение консоли. Нарушение CORS создает ошибку консоли об источнике.
    1. Некоторые проблемы CORS не могут быть решены, например, когда приложение перенаправляется на login.microsoftonline.com для проверки подлинности и срок действия маркера доступа истекает. Вызов CORS затем не удается. Обходным решением для этого сценария является продление срока действия маркера доступа, чтобы срок его действия не истекает во время сеанса пользователя. Дополнительные сведения о том, как это сделать, см. в сведениях о настраиваемых сроках действия маркеров [в платформе удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Рекомендуемые документы**

- [Настройка единого вход в прокси-приложение приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Единый вход SAML для локального приложения с помощью прокси приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Понимание и решение проблем CORS прокси приложения Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Устранение неполадок конфигураций ограниченного делегирования Kerberos для прокси приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)