---
title: Процесс разрешений и согласия API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379894"
---
# <a name="api-permissions-and-consent-process"></a>Процесс разрешений и согласия API

Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия. [В справке разрешений Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) перечислены разрешения, связанные с каждым основным набором API Microsoft Graph. В ней также приведены руководства по использованию разрешений.

**Настройка или обновление основного**

- [Создание serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) . В этой статье показано, как создать новый объект servicePrincipal.
- Создание на портале & приложения Azure [AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) — в этой статье показано, как создать новое приложение Azure Active Directory (Azure AD), которое можно использовать с помощью управления доступом на основе ролей.
- [Принципы & службы в Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) . В этой статье описываются регистрация приложений, объекты приложений и принципы службы в Azure Active Directory: что они, как они используются и как они связаны друг с другом.

**Добавление или обновление регистрации приложений и предоставление согласия администратора**

- [Создание регистрации приложения](https://docs.microsoft.com/graph/api/application-post-applications) . В этой статье показано, как создать новый объект приложения.
- [Обновление регистрации приложения - разрешения API](https://docs.microsoft.com/graph/api/application-update) . В этой статье показано, как обновить свойства объекта приложения.
- [Предоставление согласия администратора](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) . Для согласия администратора и согласия в целом, мы требуем, чтобы администратор явно дает согласие.
- [RBAC (бета-версия)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) — контейнер управления ролью для унифицированных определений ролей и назначений ролей для поставщиков Microsoft 365 RBAC, которые поддерживают несколько принципов и несколько областей в одном назначении ролей. Это отличается от типа ресурса *rbacApplication.* Microsoft Intune является примером такого поставщика RBAC. Назначение ролей в Intune может иметь массив принципалов и массив групп областей. **Это бета-версия, что означает, что она еще находится в разработке и не рекомендуется для использования в производстве.**
