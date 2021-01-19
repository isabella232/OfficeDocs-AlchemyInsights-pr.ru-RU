---
title: SamL Assertions (Tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884616"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="cb859-102">SamL Assertions (Tokens)</span><span class="sxs-lookup"><span data-stu-id="cb859-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="cb859-103">Маркеры SAML — это XML-представления утверждений.</span><span class="sxs-lookup"><span data-stu-id="cb859-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="cb859-104">По умолчанию маркеры SAML, которые Windows Communication Foundation (WCF) использует в сценариях федеративной безопасности, являются маркерами выдачи.</span><span class="sxs-lookup"><span data-stu-id="cb859-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="cb859-105">Дополнительные сведения [см. в подзаголовках маркеров и утверждений SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="cb859-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="cb859-106">Платформа удостоверений Майкрософт выдает несколько типов маркеров безопасности при обработке каждого потока проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cb859-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="cb859-107">[Справочник по утверждениям маркеров SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) описывает формат, характеристики безопасности и содержимое маркеров SAML 2.0.</span><span class="sxs-lookup"><span data-stu-id="cb859-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="cb859-108">Следуйте указаниям в настройках времени существования маркера на платформе [удостоверений Майкрософт,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) чтобы понять, как настроить время жизни маркера.</span><span class="sxs-lookup"><span data-stu-id="cb859-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="cb859-109">Выполните действия, описанные в [этой статье,](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) чтобы понять, как настроить шифрование маркеров SAML Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cb859-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="cb859-110">В Azure AD можно настроить параметры подписи сертификатов и алгоритм подписи сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cb859-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="cb859-111">Дополнительные сведения см. в дополнительных параметрах [подписи сертификатов в маркере SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)для приложений коллекции в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cb859-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
