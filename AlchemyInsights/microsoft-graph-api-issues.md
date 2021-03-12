---
title: Проблемы с API Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716205"
---
# <a name="microsoft-graph-api-issues"></a>Проблемы с API Microsoft Graph

Этот раздел также может применяться к разработчикам, использующим API Azure AD Graph. Однако настоятельно рекомендуется **использовать** Microsoft Graph для всех сценариев управления каталогом, удостоверениями и доступом.

**Проблемы с проверкой подлинности или авторизацией**

- Если ваше  приложение не может приобрести маркеры для вызова Microsoft Graph, выберите проблему с получением категории Маркер доступа **(Проверка подлинности)** Microsoft Graph, чтобы получить более конкретную помощь и поддержку по этому вопросу.
- Если ваше приложение получает **401 или 403** ошибки авторизации  при вызове Microsoft Graph, выберите категорию API API Microsoft Graph, чтобы получить более конкретную помощь и поддержку по этому вопросу.

**Я хочу использовать Microsoft Graph, но не знаю, с чего начать**

- [Обзор Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Обзор управления удостоверением и доступом в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Начало создания приложений Microsoft Graph](https://docs.microsoft.com/graph/)
- **Обозреватель Microsoft Graph** — тестирование API Microsoft Graph в клиенте или клиенте демонстрации

**Я хочу использовать Microsoft Graph, но поддерживает ли он API каталогов v1.0, которые мне нужны?**

Microsoft Graph — это рекомендуемый API для управления каталогами, удостоверением и доступом. Однако между возможными в Azure AD Graph и Microsoft Graph остаются некоторые пробелы. Просмотрите следующие статьи, в которых освещаются самые последние различия, которые помогут вам выбрать:

- [Различия типа ресурсов между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Различия свойств между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Различия метода между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, который я вызываю, не работает, где можно сделать больше тестирования?**

**Обозреватель Microsoft Graph** — проверьте API Microsoft Graph в клиенте или клиенте демонстрации, а также ознакомьтесь с примерами запросов **в** Microsoft Graph Explorer.

**Мое приложение слишком медленно и также получает регулирование. Какие улучшения можно сделать?**

В зависимости от сценария в вашем распоряжении имеется множество вариантов, которые сделают приложение более исполняемым, а в некоторых случаях менее подвержено регулированием со стороны службы (когда вы выполняете слишком много вызовов).

- [Лучшие практики Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Пакетные запросы](https://docs.microsoft.com/graph/json-batching)
- [Отслеживание изменений с помощью запроса delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Получать уведомления об изменениях через веб-сайты](https://docs.microsoft.com/graph/webhooks)
- [Руководство по регулированием](https://docs.microsoft.com/graph/throttling)

**Где можно найти дополнительные сведения об ошибках и известных проблемах?**

- [Сведения об ошибке Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Известные проблемы с Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Где можно проверить состояние доступности и подключения к службе?**

Доступность и подключение к службам, к которые можно получить доступ через Microsoft Graph, может повлиять на общую доступность и производительность Microsoft Graph.

- Чтобы проверить состояние службы Azure Active Directory, проверьте состояние служб **безопасности и** удостоверений, перечисленных на странице [состояние Azure.](https://azure.microsoft.com/status/)
- Для служб Office, которые вносят вклад в Microsoft Graph, проверьте состояние служб, перечисленных в панели мониторинга здоровья служб [Office.](https://portal.office.com/adminportal/home#/servicehealth)

Ошибки авторизации Microsoft Graph могут быть результатом нескольких различных проблем, большинство из которых создают ошибку 401 или 403. Например, ошибки авторизации могут возникнуть в результате следующих неполадок:

- Некорректные [потоки получения маркеров доступа](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Неправильно настроенные [области разрешений](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Отсутствие [согласия](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Окончание поддержки Библиотеки проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph_*)_

_*Начиная с 30 июня 2020 г.**, мы больше не будем добавлять новые функции в ADAL и Azure AD Graph. Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.

**Начиная с 30 июня 2022** г. мы переимеем поддержку ADAL и Azure AD Graph и больше не будем предоставлять техническую поддержку или обновления безопасности.

Приложения, использующие ADAL в существующих версиях ОС, продолжат работать после этого времени, но не получат никакой технической поддержки *или обновлений безопасности.*

Приложения, использующие Azure AD Graph после этого времени, могут больше не получать ответы из конечной точки Azure AD Graph.

**Миграция ADAL**

Мы рекомендуем выполнить обновление до [Библиотеки проверки подлинности Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), включающей новые возможности и обновления для системы безопасности.

Если вы используете приложения Майкрософт, знайте, что Корпорация Майкрософт в процессе переноса своих приложений в MSAL к концу срока поддержки, гарантируя, что они будут извлекать выгоду из текущих улучшений безопасности и функций MSAL.

1. [Ознакомьтесь с вопросами и ответами по ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Сведения о миграции приложений для каждой платформы](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Если вам нужна помощь в понимании того, какие из ваших приложений используют ADAL, рекомендуется просмотреть все исходные коды своих приложений, а если это применимо, связаться с любыми поставщиками isV или app. Кроме того, служба поддержки корпорации Майкрософт может предоставить вам список всех приложений сторонних разработчиков, использующих ADAL, в вашем клиенте.

**Миграция приложений, использующих AAD Graph**

Для приложений, использующих Azure AD Graph, следуйте нашим указаниям по переносу [приложений Azure AD Graph в Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Контрольный список миграции содержит стартовую точку](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. На портале регистрации приложений Azure показано, какие приложения используют AAD Graph. Рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений. Служба поддержки Майкрософт также может предоставить вам список всех данных об использовании AAD Graph в клиенте.
3. Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия. В [справке разрешений](https://docs.microsoft.com/graph/permissions-reference) Microsoft Graph перечислены разрешения, связанные с каждым основным набором API Microsoft Graph. В ней также приведены руководства по использованию разрешений.
