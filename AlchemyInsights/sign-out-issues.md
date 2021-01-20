---
title: Проблемы с выходом из учетной записи
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886899"
---
# <a name="sign-out-issues"></a><span data-ttu-id="885f8-102">Проблемы с выходом из учетной записи</span><span class="sxs-lookup"><span data-stu-id="885f8-102">Sign-out issues</span></span>

<span data-ttu-id="885f8-103">Чтобы устранить проблемы, связанные с выходом, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="885f8-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="885f8-104">Если вы или пользователь выходите или исключаетесь из приложений, следуйте инструкциям в статьях [Настройка управления сеансом проверки подлинности с помощью условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) или [Настраиваемые жизненные циклы маркеров на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="885f8-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="885f8-105">Большинство других ошибок и проблем с выходом можно решить, устраняя проблемы интеграции Azure Active Directory (Azure AD) с конкретным приложением.</span><span class="sxs-lookup"><span data-stu-id="885f8-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="885f8-106">Рекомендации по конкретно интеграции можно найти в этом [наборе руководств, посвященных интеграции приложений в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), в том числе:</span><span class="sxs-lookup"><span data-stu-id="885f8-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="885f8-107">Руководства по приложению SaaS</span><span class="sxs-lookup"><span data-stu-id="885f8-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="885f8-108">Руководства по единому входу</span><span class="sxs-lookup"><span data-stu-id="885f8-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="885f8-109">Руководства по подготовке пользователей</span><span class="sxs-lookup"><span data-stu-id="885f8-109">User-provisioning tutorials</span></span>