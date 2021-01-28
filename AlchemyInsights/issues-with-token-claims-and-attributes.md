---
title: Проблемы с утверждениями и атрибутами маркера
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029990"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="272e1-102">Проблемы с утверждениями и атрибутами маркера</span><span class="sxs-lookup"><span data-stu-id="272e1-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="272e1-103">**Обновление, настройка и удаление утверждений маркеров**</span><span class="sxs-lookup"><span data-stu-id="272e1-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="272e1-104">С помощью Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) можно настроить тип утверждения роли в маркере ответа, который вы получаете после авторизации приложения.</span><span class="sxs-lookup"><span data-stu-id="272e1-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="272e1-105">Разработчики приложений могут использовать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения они хотят использовать в маркерах, от отправленных приложению.</span><span class="sxs-lookup"><span data-stu-id="272e1-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="272e1-106">Дополнительные сведения см. в [подзагодии "Предоставление необязательных утверждений для вашего приложения".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="272e1-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="272e1-107">[Настройка групповых утверждений для приложений с помощью Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="272e1-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="272e1-108">При использовании простого единого вход в приложении см. настройки утверждений, выдаемых в [маркере SAML для корпоративных приложений.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="272e1-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="272e1-109">**Сопоставление атрибутов утверждений**</span><span class="sxs-lookup"><span data-stu-id="272e1-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="272e1-110">Чтобы настроить политику сопоставления утверждений с помощью PowerShell, см. "Настройка утверждений, выдаваемых в маркерах для определенного приложения в клиенте [(предварительная версия)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)".</span><span class="sxs-lookup"><span data-stu-id="272e1-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="272e1-111">Атрибуты расширения схемы каталогов предоставляют способ хранения дополнительных данных в Azure Active Directory для объектов пользователей и других объектов каталогов, таких как группы, сведения о клиенте, основные службы.</span><span class="sxs-lookup"><span data-stu-id="272e1-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="272e1-112">Только атрибуты расширения в объектах-пользователях можно использовать для выдания утверждений приложениям.</span><span class="sxs-lookup"><span data-stu-id="272e1-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="272e1-113">[Использование атрибутов](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) расширения схемы каталогов в утверждениях описывает использование атрибутов расширения схемы каталогов для отправки пользовательских данных приложениям в утверждениях маркеров.</span><span class="sxs-lookup"><span data-stu-id="272e1-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="272e1-114">Дополнительные сведения об утверждениях маркеров см. в:</span><span class="sxs-lookup"><span data-stu-id="272e1-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="272e1-115">Утверждения в маркерах доступа</span><span class="sxs-lookup"><span data-stu-id="272e1-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="272e1-116">Утверждения в id_token</span><span class="sxs-lookup"><span data-stu-id="272e1-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="272e1-117">[Утверждения,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) которые можно ожидать в маркерах ID и маркерах доступа, выдав azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="272e1-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="272e1-118">Справочник по утверждениям маркеров SAML</span><span class="sxs-lookup"><span data-stu-id="272e1-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
