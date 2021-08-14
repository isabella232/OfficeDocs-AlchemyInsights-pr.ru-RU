---
title: Запрос API Graph Microsoft
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923252"
---
# <a name="querying-the-microsoft-graph-api"></a>Запрос API Graph Microsoft

Этот раздел также может применяться к разработчикам, использующим API Azure AD Graph API. Однако настоятельно рекомендуется **использовать** microsoft Graph для всех сценариев управления каталогами, удостоверениями и доступом.

**Проблемы с проверкой подлинности или авторизацией**

- Если ваше  приложение не может приобрести маркеры для вызова Microsoft Graph, выберите проблему с получением маркера доступа **(проверка подлинности)** категории Microsoft Graph, чтобы получить более конкретную помощь и поддержку по этому вопросу.
- Если приложение получает **401 или 403** ошибки авторизации при вызове  Microsoft Graph, выберите категорию API Microsoft Graph получения более конкретной помощи и поддержки по этому вопросу.

**Я хочу использовать microsoft Graph, но не знаю, с чего начать**

Дополнительные информацию о microsoft Graph см. в этой записи.

- [Обзор Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Обзор управления удостоверением и доступом в Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Начало создания приложений Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** — тестирование API Graph Microsoft в клиенте или клиенте демонстрации

**Я хочу использовать microsoft Graph, но поддерживает ли он API каталога v1.0, которые мне нужны?**

Microsoft Graph — это рекомендуемый API для управления каталогами, удостоверением и доступом. Тем не менее, существует несколько пробелов между возможными в Azure AD Graph Microsoft Graph. Просмотрите следующие статьи, в которых освещаются самые последние различия, которые помогут вам выбрать:

- [Различия в типах ресурсов между Azure AD Graph и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Различия свойств между Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Различия метода между Azure AD и Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**При запросе *объекта пользователя* многие его свойства отсутствуют.**

`GET https://graph.microsoft.com/v1.0/users`возвращает только 11 свойств, так как корпорация Майкрософт Graph автоматически  выбирает набор свойств пользователя по умолчанию для возврата. Если вам нужны другие *свойства* пользователя, $select выбрать свойства, необходимые вашему приложению. Сначала попробуйте его **в Microsoft Graph Explorer.**

**Некоторые значения свойств пользователей являются *null,* хотя я знаю, что они установлены**

Наиболее вероятным объяснением является то, что приложению было предоставлено разрешение *User.ReadBasic.All.* Это позволяет приложению читать ограниченный набор свойств пользователей, возвращая все другие свойства в качестве null, даже если они были заданной ранее. Попробуйте вместо этого предоставить *приложению разрешение User.Read.All.*

Дополнительные сведения см. в [Graph разрешений пользователей.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**У меня возникли проблемы с использованием параметров запроса OData для фильтрации данных в моих запросах**

Хотя microsoft Graph поддерживает широкий диапазон параметров запроса OData, многие из этих параметров не поддерживаются полностью службами каталогов (ресурсами, наследуемыми от *directoryObject)* в Microsoft Graph. Те же ограничения, которые были в Azure AD Graph сохраняются по большей части в Microsoft Graph:

1. **Не поддерживается:**$count, $search и $filter значения *null* или *null*
2. **Не поддерживается:**$filter определенных свойств (см. разделы ресурсов, по которым свойства можно фильтровать)
3. **Не поддерживается:** одновременное фильтрация, фильтрация и сортировка
4. **Не поддерживается:** фильтрация на связи. Например, найдите всех членов инженерной группы, которые находятся в Великобритании.
5. **Частичная** поддержка: $orderby *пользователя* (только displayName и userPrincipalName) и *группы*
6. Частичная поддержка **:**$filter (поддерживает только *eq,* *startswith* *или* *,* и ( и ограничена) поддержку, $expand (расширение отношений одного объекта возвращает все отношения, но расширение коллекции отношений объектов ограничено)

Дополнительные сведения см. [в ссылке Настройка ответов с параметрами запроса.](https://docs.microsoft.com/graph/query-parameters)

**API, который я вызываю, не работает .**

**Microsoft Graph Explorer** — проверьте API microsoft Graph в клиенте или клиенте  демонстрации, а также ознакомьтесь с примерами запросов в Microsoft Graph Explorer.

**Когда я запрашиваю данные, кажется, что я получаю неполный набор данных**

Если вы запрашиваете коллекцию (например, *пользователей),* microsoft Graph использует ограничения страниц на стороне сервера, чтобы результаты всегда возвращались с размером страницы по умолчанию. Ваше приложение всегда должно рассчитывать на страницу через коллекции, возвращенные из службы.

Дополнительные сведения см. в указанных ниже статьях.

- [Лучшие Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Разбиение данных Microsoft Graph по страницам в приложении](https://docs.microsoft.com/graph/paging)

**Мое приложение слишком медленно и также получает регулирование. Какие улучшения можно сделать?**

В зависимости от сценария в вашем распоряжении имеется множество различных вариантов, чтобы сделать приложение более исполняемым, а в некоторых случаях менее подвержено регулированием со стороны службы (когда вы выполняете слишком много вызовов).

Дополнительные сведения см. в статьях

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
