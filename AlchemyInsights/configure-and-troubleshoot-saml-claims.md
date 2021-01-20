---
title: Настройка утверждений SAML и устранение неполадок
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
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886896"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="c19d5-102">Настройка утверждений SAML и устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="c19d5-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="c19d5-103">Для настройки утверждений SAML и устранения неполадок:</span><span class="sxs-lookup"><span data-stu-id="c19d5-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="c19d5-104">Выполните действия, описанные в [этой статье](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management), чтобы настроить утверждение роли, выданное в маркере SAML для корпоративных приложений.</span><span class="sxs-lookup"><span data-stu-id="c19d5-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="c19d5-105">Выполните действия, описанные в [этой статье](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization), чтобы настроить утверждения, выпущенные в маркере SAML для корпоративных приложений.</span><span class="sxs-lookup"><span data-stu-id="c19d5-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="c19d5-106">Выполните действия, описанные в [этой статье](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping), чтобы настроить утверждения, выпущенные в маркерах для конкретного приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c19d5-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="c19d5-107">Узнать, как работать с приложениями с поддержкой утверждений в прокси-приложении можно из [этой статьи](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications).</span><span class="sxs-lookup"><span data-stu-id="c19d5-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>