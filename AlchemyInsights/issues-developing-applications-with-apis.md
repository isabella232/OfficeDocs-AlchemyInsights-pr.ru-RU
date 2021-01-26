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
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="30a4b-102">Проблемы разработки приложений с помощью API</span><span class="sxs-lookup"><span data-stu-id="30a4b-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="30a4b-103">Чтобы начать использовать API Graph Azure Active Directory, см. краткое руководство по [API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) или интерактивную справочную документацию по [API Azure AD Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="30a4b-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="30a4b-104">**Окончание поддержки библиотеки проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="30a4b-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="30a4b-105">**С 30 июня 2020** г. мы больше не добавим новые функции в ADAL и Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="30a4b-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="30a4b-106">Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления функций.</span><span class="sxs-lookup"><span data-stu-id="30a4b-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="30a4b-107">**Начиная с 30 июня 2022** г., поддержка ADAL и Azure AD Graph будет прекратиться, и мы больше не будем предоставлять техническую поддержку или обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="30a4b-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="30a4b-108">Приложения, использующие ADAL в существующих версиях ОС, продолжат работать после этого времени, но не будут получать техническую поддержку или обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="30a4b-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="30a4b-109">Приложения, использующие Azure AD Graph после этого времени, больше не будут получать ответы от конечной точки Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="30a4b-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="30a4b-110">**Миграция ADAL**</span><span class="sxs-lookup"><span data-stu-id="30a4b-110">**ADAL Migration**</span></span>

<span data-ttu-id="30a4b-111">Рекомендуем обновить библиотеку проверки подлинности [Майкрософт (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)с последними функциями и обновлениями для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="30a4b-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="30a4b-112">Если вы используете приложения Майкрософт, необходимо знать, что корпорация Майкрософт находится в процессе переноса своих приложений в MSAL к крайнему сроку поддержки, обеспечивая им преимущества от текущих улучшений безопасности и функций MSAL.</span><span class="sxs-lookup"><span data-stu-id="30a4b-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="30a4b-113">[Ознакомьтесь с ADAL: faq](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="30a4b-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="30a4b-114">[Узнайте, как перенести приложения для разных платформ.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="30a4b-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="30a4b-115">Если вам нужна помощь в понимании того, какое из ваших приложений использует ADAL, рекомендуем просмотреть весь исходный код своих приложений и, если применимо, связаться с любыми поставщиками программного обеспечения или поставщиками приложений.</span><span class="sxs-lookup"><span data-stu-id="30a4b-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="30a4b-116">Служба поддержки Майкрософт также может предоставить вам список всех приложений, не в том числе ADAL от Майкрософт, в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="30a4b-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="30a4b-117">**Миграция AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="30a4b-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="30a4b-118">Для приложений, использующих Azure AD Graph, следуйте нашим рекомендациям по переносу приложений [Azure AD Graph в Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="30a4b-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="30a4b-119">[Наш контрольный список миграции предоставляет точку начала работы.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="30a4b-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="30a4b-120">На портале регистрации приложений Azure показано, какие приложения используют AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="30a4b-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="30a4b-121">Рекомендуем просмотреть все исходные коды приложений и, если применимо, связаться с любыми поставщиками программного обеспечения или поставщиками приложений.</span><span class="sxs-lookup"><span data-stu-id="30a4b-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="30a4b-122">Служба поддержки Майкрософт также может предоставить вам список всех данных об использовании AAD Graph в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="30a4b-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="30a4b-123">Чтобы приложение имело доступ к данным в Microsoft Graph, пользователь или администратор должен предоставить ему соответствующие разрешения с помощью процедуры получения согласия.</span><span class="sxs-lookup"><span data-stu-id="30a4b-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="30a4b-124">В [справочнике по разрешениям Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) перечислены разрешения, связанные с каждым основным набором API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30a4b-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="30a4b-125">В ней также приведены руководства по использованию разрешений.</span><span class="sxs-lookup"><span data-stu-id="30a4b-125">It also provides guidance about how to use the permissions.</span></span>
