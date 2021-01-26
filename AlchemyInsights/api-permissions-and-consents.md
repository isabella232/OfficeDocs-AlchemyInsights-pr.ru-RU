---
title: Разрешения и согласие API
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951921"
---
# <a name="api-permissions-and-consent"></a>Разрешения и согласие API

Приложения, которые интегрируются с платформой удостоверений Майкрософт, следуют модели авторизации, которая позволяет пользователям и администраторам управлять доступом к данным. Реализация модели авторизации обновлена в конечной точке платформы удостоверений Майкрософт. Он изменяет то, как приложение должно взаимодействовать с платформой удостоверений Майкрософт. [Разрешения и согласие в конечной](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) точке платформы удостоверений Майкрософт охватывают основные понятия этой модели авторизации, включая области, разрешения и согласие.

Платформа [согласия Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) упрощает разработку многоязычных веб-приложений и нативных клиентских приложений. Эти приложения позволяют войти с помощью учетных записей пользователей из клиента Azure AD, который отличается от того, в котором зарегистрировано приложение. Кроме того, им может потребоваться доступ к веб-API, таким как API Microsoft Graph (для доступа к Azure AD, Intune и службам в Microsoft 365) и другим API служб Майкрософт, а также к собственным веб-API.

