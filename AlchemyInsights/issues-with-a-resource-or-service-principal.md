---
title: Проблемы с директором ресурса или службы
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028089"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Проблемы с директором ресурса или службы

1. Если вы только начинаете работу, основные объекты приложений и служб в [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) описывают регистрацию приложений, объекты приложений и принципы обслуживания в Azure Active Directory: что они, как они используются и как они связаны друг с другом. Кроме того, представлен сценарий с несколькими клиентами, чтобы проиллюстрировать связь между объектом приложения приложения и соответствующими основными объектами службы.
2. Вы можете узнать больше об отношениях между приложениями и директорами служб, прочитав приложения и основные объекты [службы в Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Использование портала для создания приложения и основной [службы Azure AD,](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) которые могут получать доступ к ресурсам, показывает, как создать новое приложение Azure Active Directory Azure AD и главу службы, которые можно использовать с помощью управления доступом на основе ролей.
4. С помощью [главного API службы](https://docs.microsoft.com/graph/api/resources/serviceprincipal)можно программным образом управлять экземплярами приложений и управлять тем, что приложение может сделать в клиенте.
5. [Тип ресурса servicePrincipal перечисляет](https://docs.microsoft.com/graph/api/resources/serviceprincipal) все свойства и методы для типа ресурса servicePrincipal.
6. [Различия в типах](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) ресурсов между Azure AD Graph и Microsoft Graph подчеркивают различия между ресурсами Azure AD Graph и Microsoft Graph. В нем показаны ресурсы с разными именами или недоступными; он также выделяет ресурсы, доступные в бета-версии Microsoft Graph, но не в версии v1.0.

**Проблемы с гостевых пользователей**

- [Quickstart.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Добавление гостевых пользователей в каталог на портале Azure показывает, как добавить нового гостевых пользователей в каталог Azure AD через портал Azure, отправить приглашение и узнать, как выглядит процесс выкупа приглашений гостевого пользователя.
- [Руководство. Создание потоков пользователей в Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) показывает, как создать некоторые рекомендуемые потоки пользователей с помощью портала Azure. Если вы ищете сведения о настройке потока учетных данных владельца ресурса (ROPC) в вашем приложении, см. в приложении Configure the resource owner password credentials flow in Azure AD B2C.
