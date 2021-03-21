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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="de316-102">Устранение неполадок с кодами ошибок аутентификации и авторизации Azure AD (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="de316-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="de316-103">Чтобы устранить ошибки аутентификации и авторизации AAD (AADSTS), выполните следующие рекомендуемые действия.</span><span class="sxs-lookup"><span data-stu-id="de316-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="de316-104">**Обработка кодов ошибок в приложении**</span><span class="sxs-lookup"><span data-stu-id="de316-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="de316-105">В **спецификации OAuth2.0** (https://tools.ietf.org/html/rfc6749#section-5.2) представлены инструкции по устранению ошибок при проверке подлинности с использованием части сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="de316-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="de316-106">**error**: строка кода ошибки, которую можно использовать для классификации типов ошибок и следует использовать для реагирования на ошибки.</span><span class="sxs-lookup"><span data-stu-id="de316-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="de316-107">Поле **error** может иметь несколько возможных значений. Дополнительные сведения о конкретных ошибках и реагировании на них можно найти по ссылкам на документацию по протоколу и в спецификациях OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="de316-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="de316-108">Это пример сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="de316-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="de316-109">**Поиск текущих сведений о коде ошибки**</span><span class="sxs-lookup"><span data-stu-id="de316-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="de316-110">Коды ошибок и сообщения о них могут меняться.</span><span class="sxs-lookup"><span data-stu-id="de316-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="de316-111">Самые свежие сведения можно найти на странице https://login.microsoftonline.com/error с описанием ошибок AADSTS, способами их устранения и рекомендуемыми обходными решениями.</span><span class="sxs-lookup"><span data-stu-id="de316-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="de316-112">Также можно использовать [коды ошибок AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes), указанные в статье [Коды ошибок аутентификации и авторизации Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="de316-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="de316-113">**Получение помощи**</span><span class="sxs-lookup"><span data-stu-id="de316-113">**Get Help**</span></span>

- <span data-ttu-id="de316-114">[Возможности получения поддержки и помощи для разработчиков](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options). Если вам нужен ответ на вопрос или помощь в решении проблемы, не описанной в нашей документации, возможно, пришло время обратиться за помощью к специалистам.</span><span class="sxs-lookup"><span data-stu-id="de316-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="de316-115">В этой статье предлагается несколько вариантов получения ответов на ваши вопросы при разработке приложений, которые интегрируются с платформой удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="de316-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>







