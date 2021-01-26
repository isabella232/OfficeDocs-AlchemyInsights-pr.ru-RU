---
title: Проблемы при разработке приложений
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950800"
---
# <a name="issues-developing-applications"></a>Проблемы при разработке приложений

Чтобы устранить наиболее распространенные проблемы при создании приложений Azure Active Directory (AD), см. следующие статьи:

- [Возникли проблемы с входом в приложения: только с помощью браузера Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Не знаю, как изменить значение по умолчанию времени существования маркера для моего приложения](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Не могу понять, как работает согласие с условиями приложения](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Не знаю, как предоставить разрешения для моего приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Не понимаю, в чем разница между делегированными разрешениями и разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Окончание поддержки Библиотеки проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph)** _

- С 30 июня 2020 г. мы больше не будем добавлять новые возможности в Библиотеку проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph). Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.

- С 30 июня 2022 г. мы завершаем поддержку ADAL и AAD Graph и больше не будем предоставлять техническую поддержку и обновления для системы безопасности. Это подразумевает следующее:

    - Приложения, использующие ADAL в существующих версиях ОС, будут по-прежнему работать после этой даты, но им не будет предоставляться техническая поддержка и обновления для системы безопасности.

    - Приложения, использующие AAD Graph после этой даты, больше не будут получать ответы от конечной точки AAD Graph.

_ *Миграция приложений, использующих ADAL**

Если вы используете приложения Майкрософт, рекомендуем выполнить обновление до Библиотеки проверки подлинности Microsoft (MSAL), включающей новые возможности и обновления для системы безопасности. Эта рекомендация дается в контексте инициирования корпорацией Майкрософт процесса миграции ее приложений в MSAL к дате окончания поддержки. 

Миграция приложений Майкрософт в MSAL обеспечивает применение текущих улучшений системы безопасности и компонентов MSAL в приложениях.

1. [Ознакомьтесь с вопросами и ответами по ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Сведения о миграции приложений для каждой платформы](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Если вам нужна помощь, чтобы понять, которые из ваших приложений используют ADAL, рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений. Кроме того, служба поддержки Microsoft может предоставить вам список всех приложений сторонних разработчиков, использующих ADAL, в вашем клиенте.

**Миграция приложений, использующих AAD Graph**

Следуйте нашему руководству, что перенести приложения, использующие AAD Graph, в Microsoft Graph:

1. [Контрольный список миграции содержит стартовую точку](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. На портале регистрации приложений Azure показано, какие приложения используют AAD Graph. Рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений. Кроме того, служба поддержки Microsoft может предоставить вам сведения об использовании AAD Graph в вашем клиенте.







