---
title: Проблемы разработки приложений с помощью API
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951927"
---
# <a name="issues-developing-applications-with-apis"></a>Проблемы разработки приложений с помощью API

Чтобы начать использовать API Graph Azure Active Directory, см. краткое руководство по [API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) или интерактивную справочную документацию по [API Azure AD Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Окончание поддержки библиотеки проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph)**

**С 30 июня 2020** г. мы больше не добавим новые функции в ADAL и Azure AD Graph. Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления функций.

**Начиная с 30 июня 2022** г., поддержка ADAL и Azure AD Graph будет прекратиться, и мы больше не будем предоставлять техническую поддержку или обновления для системы безопасности.

Приложения, использующие ADAL в существующих версиях ОС, продолжат работать после этого времени, но не будут получать техническую поддержку или обновления для системы безопасности.

Приложения, использующие Azure AD Graph после этого времени, больше не будут получать ответы от конечной точки Azure AD Graph.

**Миграция ADAL**

Рекомендуем обновить библиотеку проверки подлинности [Майкрософт (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)с последними функциями и обновлениями для системы безопасности.

Если вы используете приложения Майкрософт, необходимо знать, что корпорация Майкрософт находится в процессе переноса своих приложений в MSAL к крайнему сроку поддержки, обеспечивая им преимущества от текущих улучшений безопасности и функций MSAL.

1. [Ознакомьтесь с ADAL: faq](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Узнайте, как перенести приложения для разных платформ.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Если вам нужна помощь в понимании того, какое из ваших приложений использует ADAL, рекомендуем просмотреть весь исходный код своих приложений и, если применимо, связаться с любыми поставщиками программного обеспечения или поставщиками приложений. Служба поддержки Майкрософт также может предоставить вам список всех приложений, не в том числе ADAL от Майкрософт, в вашем клиенте.

**Миграция AAD Graph**

Для приложений, использующих Azure AD Graph, следуйте нашим рекомендациям по переносу приложений [Azure AD Graph в Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Наш контрольный список миграции предоставляет точку начала работы.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. На портале регистрации приложений Azure показано, какие приложения используют AAD Graph. Рекомендуем просмотреть все исходные коды приложений и, если применимо, связаться с любыми поставщиками программного обеспечения или поставщиками приложений. Служба поддержки Майкрософт также может предоставить вам список всех данных об использовании AAD Graph в вашем клиенте.
1. Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия. В [справочнике по разрешениям Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) перечислены разрешения, связанные с каждым основным набором API Microsoft Graph. В ней также приведены руководства по использованию разрешений.
