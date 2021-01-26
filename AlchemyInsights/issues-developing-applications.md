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
# <a name="issues-developing-applications"></a><span data-ttu-id="8e8cc-102">Проблемы при разработке приложений</span><span class="sxs-lookup"><span data-stu-id="8e8cc-102">Issues developing applications</span></span>

<span data-ttu-id="8e8cc-103">Чтобы устранить наиболее распространенные проблемы при создании приложений Azure Active Directory (AD), см. следующие статьи:</span><span class="sxs-lookup"><span data-stu-id="8e8cc-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="8e8cc-104">Возникли проблемы с входом в приложения: только с помощью браузера Chrome</span><span class="sxs-lookup"><span data-stu-id="8e8cc-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="8e8cc-105">Не знаю, как изменить значение по умолчанию времени существования маркера для моего приложения</span><span class="sxs-lookup"><span data-stu-id="8e8cc-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="8e8cc-106">Не могу понять, как работает согласие с условиями приложения</span><span class="sxs-lookup"><span data-stu-id="8e8cc-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="8e8cc-107">Не знаю, как предоставить разрешения для моего приложения</span><span class="sxs-lookup"><span data-stu-id="8e8cc-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="8e8cc-108">Не понимаю, в чем разница между делегированными разрешениями и разрешениями приложений</span><span class="sxs-lookup"><span data-stu-id="8e8cc-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="8e8cc-109">\***Окончание поддержки Библиотеки проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="8e8cc-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="8e8cc-110">С 30 июня 2020 г. мы больше не будем добавлять новые возможности в Библиотеку проверки подлинности Azure Active Directory (ADAL) и API Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="8e8cc-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="8e8cc-111">Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="8e8cc-112">С 30 июня 2022 г. мы завершаем поддержку ADAL и AAD Graph и больше не будем предоставлять техническую поддержку и обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="8e8cc-113">Это подразумевает следующее:</span><span class="sxs-lookup"><span data-stu-id="8e8cc-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="8e8cc-114">Приложения, использующие ADAL в существующих версиях ОС, будут по-прежнему работать после этой даты, но им не будет предоставляться техническая поддержка и обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="8e8cc-115">Приложения, использующие AAD Graph после этой даты, больше не будут получать ответы от конечной точки AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="8e8cc-116">_ *Миграция приложений, использующих ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="8e8cc-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="8e8cc-117">Если вы используете приложения Майкрософт, рекомендуем выполнить обновление до Библиотеки проверки подлинности Microsoft (MSAL), включающей новые возможности и обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="8e8cc-118">Эта рекомендация дается в контексте инициирования корпорацией Майкрософт процесса миграции ее приложений в MSAL к дате окончания поддержки.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="8e8cc-119">Миграция приложений Майкрософт в MSAL обеспечивает применение текущих улучшений системы безопасности и компонентов MSAL в приложениях.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="8e8cc-120">Ознакомьтесь с вопросами и ответами по ADAL</span><span class="sxs-lookup"><span data-stu-id="8e8cc-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="8e8cc-121">Сведения о миграции приложений для каждой платформы</span><span class="sxs-lookup"><span data-stu-id="8e8cc-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="8e8cc-122">Если вам нужна помощь, чтобы понять, которые из ваших приложений используют ADAL, рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="8e8cc-123">Кроме того, служба поддержки Microsoft может предоставить вам список всех приложений сторонних разработчиков, использующих ADAL, в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8e8cc-124">**Миграция приложений, использующих AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="8e8cc-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="8e8cc-125">Следуйте нашему руководству, что перенести приложения, использующие AAD Graph, в Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8e8cc-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="8e8cc-126">[Контрольный список миграции содержит стартовую точку](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="8e8cc-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="8e8cc-127">На портале регистрации приложений Azure показано, какие приложения используют AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8e8cc-128">Рекомендуем просмотреть исходный код всех приложений и, если возможно, связаться с независимыми поставщиками программного обеспечения (ISV) или поставщиками приложений.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="8e8cc-129">Кроме того, служба поддержки Microsoft может предоставить вам сведения об использовании AAD Graph в вашем клиенте.</span><span class="sxs-lookup"><span data-stu-id="8e8cc-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







