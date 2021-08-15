---
title: Проблемы разработки приложений с API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013473"
---
# <a name="issues-developing-applications-with-apis"></a>Проблемы разработки приложений с API

Чтобы начать использовать API Azure Active Directory Graph, см. руководство по быстрой подготовке Graph [API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) Azure AD или интерактивную справочную документацию по API azure [AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Завершение поддержки библиотеки Azure Active Directory проверки подлинности (ADAL) и API Azure AD Graph API (AAD Graph)**

**Начиная с 30 июня 2020** г. мы больше не будем добавлять новые функции в ADAL и Azure AD Graph. Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.

**Начиная с 30 июня 2022** г. мы перезахолим поддержку ADAL и Azure AD Graph и больше не будем предоставлять техническую поддержку или обновления безопасности.

Приложения, использующие ADAL в существующих версиях ОС, будут по-прежнему работать после этой даты, но им не будет предоставляться техническая поддержка и обновления для системы безопасности.

Приложения, использующие Azure AD Graph после этой даты, больше не будут получать ответы от конечной точки Azure AD Graph.

**Миграция ADAL**

Мы рекомендуем выполнить обновление до [Библиотеки проверки подлинности Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), включающей новые возможности и обновления для системы безопасности.

Если вы используете приложения Майкрософт, знайте, что Корпорация Майкрософт в процессе переноса своих приложений в MSAL к концу срока поддержки, гарантируя, что они будут извлекать выгоду из текущих улучшений безопасности и функций MSAL.

1. [Ознакомьтесь с вопросами и ответами по ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Сведения о миграции приложений для каждой платформы](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Если вам нужна помощь в понимании того, какие из ваших приложений используют ADAL, рекомендуется просмотреть все исходные коды своих приложений, а если это применимо, связаться с любыми поставщиками isV или app. Кроме того, служба поддержки корпорации Майкрософт может предоставить вам список всех приложений сторонних разработчиков, использующих ADAL, в вашем клиенте.

**Миграция приложений, использующих AAD Graph**

Для приложений, использующих Azure AD Graph, следуйте нашим указаниям по переносу приложений [Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)в Microsoft Graph.

1. [Контрольный список миграции содержит стартовую точку](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. На портале регистрации приложений Azure показано, какие приложения используют AAD Graph. Рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений. Служба поддержки Майкрософт также может предоставить вам список всех Graph AAD в клиенте.
1. Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия. В [справочнике Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) майкрософт перечислены разрешения, связанные с каждым основным набором API Graph Microsoft. В ней также приведены руководства по использованию разрешений.
