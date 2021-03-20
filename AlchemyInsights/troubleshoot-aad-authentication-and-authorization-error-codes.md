---
title: Устранение неполадок с кодами ошибок аутентификации и авторизации Azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898312"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Устранение неполадок с кодами ошибок аутентификации и авторизации Azure AD (AADSTS)

Чтобы устранить ошибки аутентификации и авторизации AAD (AADSTS), выполните следующие рекомендуемые действия.

1. **Обработка кодов ошибок в приложении**

- В **спецификации OAuth2.0** (https://tools.ietf.org/html/rfc6749#section-5.2) представлены инструкции по устранению ошибок при проверке подлинности с использованием части сообщения об ошибке.

    - **error**: строка кода ошибки, которую можно использовать для классификации типов ошибок и следует использовать для реагирования на ошибки.
    - Поле **error** может иметь несколько возможных значений. Дополнительные сведения о конкретных ошибках и реагировании на них можно найти по ссылкам на документацию по протоколу и в спецификациях OAuth 2.0.

- Это пример сообщения об ошибке.
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Поиск текущих сведений о коде ошибки**

- Коды ошибок и сообщения о них могут меняться. Самые свежие сведения можно найти на странице https://login.microsoftonline.com/error с описанием ошибок AADSTS, способами их устранения и рекомендуемыми обходными решениями.
- Также можно использовать [коды ошибок AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes), указанные в статье [Коды ошибок аутентификации и авторизации Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Получение помощи**

- [Возможности получения поддержки и помощи для разработчиков](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options). Если вам нужен ответ на вопрос или помощь в решении проблемы, не описанной в нашей документации, возможно, пришло время обратиться за помощью к специалистам. В этой статье предлагается несколько вариантов получения ответов на ваши вопросы при разработке приложений, которые интегрируются с платформой удостоверений Майкрософт.








