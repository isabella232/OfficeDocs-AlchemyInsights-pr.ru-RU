---
title: Запрос aPI Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950778"
---
# <a name="querying-the-microsoft-graph-api"></a>Запрос aPI Microsoft Graph

Этот раздел также может быть применим к разработчикам, которые по-прежнему используют API Azure AD Graph. Однако настоятельно рекомендуется **использовать** Microsoft Graph для всех сценариев управления каталогом, удостоверениями и доступом.

**Проблемы с проверкой подлинности или авторизацией**

- Если приложению  не удается получить маркеры для вызова Microsoft Graph, выберите "Проблема с получением категории маркера доступа **(аутентификации)** Microsoft Graph", чтобы получить более подробную справку и поддержку в этом разделе.
- Если ваше приложение получает ошибки авторизации **401 или 403** при вызове Microsoft Graph, выберите категорию API Microsoft Graph "Получение ошибки в доступе отказано в доступе (авторизация"), чтобы получить более подробную справку и поддержку по этому разделу. 

**Я хочу использовать Microsoft Graph, но не знаю, с чего начать**

Дополнительные данные о Microsoft Graph см. в:

- [Обзор Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Обзор управления удостоверением и доступом в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Начало создания приложений Microsoft Graph](https://docs.microsoft.com/graph/)
- **Обозреватель Microsoft Graph:** тестирование API Microsoft Graph в клиенте или демонстрационных клиентах

**Я хочу использовать Microsoft Graph, но поддерживает ли он необходимые API каталогов v1.0?**

Microsoft Graph — это рекомендуемый API для управления каталогом, удостоверением и доступом. Однако между возможными в Azure AD Graph и Microsoft Graph пробелами по-прежнему существует. Просмотрите следующие статьи, в которых рассматриваются самые последние отличия, которые помогут вам в выборе:

- [Различия между типами ресурсов между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Различия свойств между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Различия методов между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**При запросе *объекта пользователя* многие его свойства отсутствуют**

`GET https://graph.microsoft.com/v1.0/users`Возвращает только 11 свойств, так как Microsoft Graph автоматически  выбирает набор свойств пользователя по умолчанию для возврата. Если вам нужны другие *свойства* пользователя, используйте $select, чтобы выбрать свойства, необходимые приложению. Сначала попробуйте его в **microsoft Graph Explorer.**

**Некоторые значения свойств пользователя имеют *значение NULL,* хотя я знаю, что они установлены**

Наиболее вероятным объяснением является то, что приложению было предоставлено разрешение *User.ReadBasic.All.* Это позволяет приложению считывать ограниченный набор свойств пользователя, возвращая все остальные свойства в качестве null, даже если они были заданной ранее. Попробуйте предоставить приложению *разрешение User.Read.All.*

Дополнительные сведения см. в [сведениях о разрешениях пользователей Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**У меня возникли проблемы с использованием параметров запросов OData для фильтрации данных в моих запросах**

Хотя Microsoft Graph поддерживает широкий спектр параметров запросов OData, многие из этих параметров не полностью поддерживаются службами каталогов (ресурсами, наследующий от *directoryObject)* в Microsoft Graph. Те же ограничения, которые присутствуют в Azure AD Graph, по большей части сохраняются в Microsoft Graph:

1. **Не поддерживается:**$count, $search и $filter значений *null* или *null*
2. **Не поддерживается:**$filter для определенных свойств (см. разделы о ресурсах, по которым можно фильтровать свойства)
3. **Не поддерживается:** одновременное разгона, фильтрация и сортировка
4. **Не поддерживается:** фильтрация по отношениям. Например, найдите всех членов инженерной группы, которые находятся в Соединенном Королевстве.
5. **Частичная** поддержка: $orderby *пользователя* (только displayName и userPrincipalName) и *группы*
6. Частичная **поддержка:**$filter (поддерживает только *eq,* *startswith,* или *,* и *,* и ограниченную *любую)* поддержку, $expand (расширение связей одного объекта возвращает все связи, но расширение коллекции связей объектов ограничено)

Дополнительные сведения [см. в подстройке ответов с помощью параметров запроса.](https://docs.microsoft.com/graph/query-parameters)

**API, который я вызываю, не работает— где можно больше тестировать?**

**Microsoft Graph Explorer:** тестирование API Microsoft Graph в клиенте  или демонстрационных клиентах, а также примеры запросов в проводнике Microsoft Graph.

**При запросе данных кажется, что возвращается неполный набор данных**

Если вы запрашиваете коллекцию (например, *пользователей),* Microsoft Graph использует ограничения страниц на стороне сервера, чтобы результаты всегда возвращались с размером страницы по умолчанию. Ваше приложение должно всегда рассчитывать на страницу с помощью коллекций, возвращаемой службой.

Дополнительные сведения см. в указанных ниже статьях.

- [Лучшие методики Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Разбиение данных Microsoft Graph по страницам в приложении](https://docs.microsoft.com/graph/paging)

**Мое приложение работает слишком медленно и также получает регулирование. Какие улучшения можно внести?**

В зависимости от вашего сценария в вашем распоряжении имеется множество различных вариантов, чтобы сделать приложение более емким и в некоторых случаях менее подвержено регулированием службой (когда выполняется слишком много вызовов).

Дополнительные сведения см. в статьях

- [Лучшие методики Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Пакетные запросы](https://docs.microsoft.com/graph/json-batching)
- [Отслеживание изменений с помощью запроса изменений](https://docs.microsoft.com/graph/delta-query-overview)
- [Получать уведомления об изменениях через веб-hooks](https://docs.microsoft.com/graph/webhooks)
- [Руководство по регулированием](https://docs.microsoft.com/graph/throttling)

**Где можно найти дополнительные сведения об ошибках и известных проблемах?**

- [Сведения об ошибке Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Известные проблемы с Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Где можно проверить состояние доступности и подключения службы?**

Доступность и подключение служб, к которые можно получить доступ через Microsoft Graph, может повлиять на общую доступность и производительность Microsoft Graph.

- Для проверки состояния службы Azure Active Directory проверьте состояние служб безопасности **и** удостоверений, перечисленных на странице [состояния Azure.](https://azure.microsoft.com/status/)
- Для служб Office, которые внесли свой вклад в Microsoft Graph, проверьте состояние служб, перечисленных в панели мониторинга состояния служб [Office.](https://portal.office.com/adminportal/home#/servicehealth)
