---
title: Проблемы Graph API Майкрософт
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975906"
---
# <a name="microsoft-graph-api-issues"></a>Проблемы Graph API Майкрософт

Этот раздел также может применяться к разработчикам, использующим API Azure AD Graph API. Однако настоятельно рекомендуется **использовать** microsoft Graph для всех сценариев управления каталогами, удостоверениями и доступом.

**Проблемы с проверкой подлинности или авторизацией**

- Если ваше  приложение не может приобрести маркеры для вызова Microsoft Graph, выберите проблему с получением маркера доступа **(проверка подлинности)** категории Microsoft Graph, чтобы получить более конкретную помощь и поддержку по этому вопросу.
- Если приложение получает **401 или 403** ошибки авторизации при вызове  Microsoft Graph, выберите категорию API Microsoft Graph получения более конкретной помощи и поддержки по этому вопросу.

**Я хочу использовать microsoft Graph, но не знаю, с чего начать**

- [Обзор Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Обзор управления удостоверением и доступом в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Начало создания приложений Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** — тестирование API Graph Microsoft в клиенте или клиенте демонстрации

**Я хочу использовать microsoft Graph, но поддерживает ли он API каталога v1.0, которые мне нужны?**

Microsoft Graph — это рекомендуемый API для управления каталогами, удостоверением и доступом. Тем не менее, существует несколько пробелов между возможными в Azure AD Graph Microsoft Graph. Просмотрите следующие статьи, в которых освещаются самые последние различия, которые помогут вам выбрать:

- [Различия в типах ресурсов между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Различия свойств между Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Различия метода между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, который я вызываю, не работает, где можно сделать больше тестирования?**

**Microsoft Graph Explorer** — проверьте API microsoft Graph в клиенте или клиенте  демонстрации, а также ознакомьтесь с примерами запросов в Microsoft Graph Explorer.

**Мое приложение слишком медленно и также получает регулирование. Какие улучшения можно сделать?**

В зависимости от сценария в вашем распоряжении имеется множество вариантов, которые сделают приложение более исполняемым, а в некоторых случаях менее подвержено регулированием со стороны службы (когда вы выполняете слишком много вызовов).

- [Лучшие Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Пакетные запросы](https://docs.microsoft.com/graph/json-batching)
- [Отслеживание изменений с помощью запроса delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Получать уведомления об изменениях через веб-сайты](https://docs.microsoft.com/graph/webhooks)
- [Руководство по регулированием](https://docs.microsoft.com/graph/throttling)

**Где можно найти дополнительные сведения об ошибках и известных проблемах?**

- [Сведения Graph ответа на ошибки](https://docs.microsoft.com/graph/errors)
- [Известные проблемы с Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Где можно проверить состояние доступности и подключения к службе?**

Доступность и подключение к службам, к которые можно получить доступ через Microsoft Graph, может повлиять на общую доступность и производительность microsoft Graph.

- Для Azure Active Directory службы проверьте состояние служб **безопасности и** удостоверений, перечисленных на странице Состояние [Azure.](https://azure.microsoft.com/status/)
- Для Office служб, которые вносят вклад в microsoft Graph, проверьте состояние служб, перечисленных в панели мониторинга Office [службы.](https://portal.office.com/adminportal/home#/servicehealth)

Ошибки Graph майкрософт могут быть результатом нескольких различных проблем, большинство из которых создают ошибку 401 или 403. Например, ошибки авторизации могут возникнуть в результате следующих неполадок:

- Некорректные [потоки получения маркеров доступа](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Неправильно настроенные [области разрешений](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Отсутствие [согласия](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Завершение поддержки библиотеки Azure Active Directory проверки подлинности (ADAL) и API Azure AD Graph API (AAD Graph)***

**Начиная с 30 июня 2020** г. мы больше не будем добавлять новые функции в ADAL и Azure AD Graph. Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.

**Начиная с 30 июня 2022** г. мы перезахолим поддержку ADAL и Azure AD Graph и больше не будем предоставлять техническую поддержку или обновления безопасности.

Приложения, использующие ADAL в существующих версиях ОС, будут по-прежнему работать после этой даты, но им *не будет предоставляться техническая поддержка и обновления для системы безопасности*.

Приложения, использующие Azure AD Graph после этой даты, больше не будут получать ответы от конечной точки Azure AD Graph.

**Миграция ADAL**

Мы рекомендуем выполнить обновление до [Библиотеки проверки подлинности Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), включающей новые возможности и обновления для системы безопасности.

Если вы используете приложения Майкрософт, знайте, что Корпорация Майкрософт в процессе переноса своих приложений в MSAL к концу срока поддержки, гарантируя, что они будут извлекать выгоду из текущих улучшений безопасности и функций MSAL.

1. [Ознакомьтесь с вопросами и ответами по ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Сведения о миграции приложений для каждой платформы](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Если вам нужна помощь в понимании того, какие из ваших приложений используют ADAL, рекомендуется просмотреть все исходные коды своих приложений, а если это применимо, связаться с любыми поставщиками isV или app. Кроме того, служба поддержки корпорации Майкрософт может предоставить вам список всех приложений сторонних разработчиков, использующих ADAL, в вашем клиенте.

**Миграция приложений, использующих AAD Graph**

Для приложений, использующих Azure AD Graph, следуйте нашим указаниям по переносу приложений [Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)в Microsoft Graph.

1. [Контрольный список миграции содержит стартовую точку](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. На портале регистрации приложений Azure показано, какие приложения используют AAD Graph. Рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений. Служба поддержки Майкрософт также может предоставить вам список всех Graph AAD в клиенте.
3. Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия. В [справочнике Graph](https://docs.microsoft.com/graph/permissions-reference) майкрософт перечислены разрешения, связанные с каждым основным набором API Graph Microsoft. В ней также приведены руководства по использованию разрешений.
