---
title: Конфигурация прокси приложения
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876561"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="f06b6-102">Конфигурация прокси приложения</span><span class="sxs-lookup"><span data-stu-id="f06b6-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="f06b6-103">Чтобы понять, как настроить приложение-прокси приложения в Azure AD для того, чтобы ваши приложения были в облаке, см. статью "Настройка приложения-прокси [приложения".](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="f06b6-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="f06b6-104">Единый вход позволяет пользователям получать доступ к приложению без многократной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f06b6-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="f06b6-105">Он позволяет выполнить одну проверку подлинности в облаке в Azure Active Directory и позволяет службе или соединителу подает пользователя на дополнительные задачи проверки подлинности из приложения.</span><span class="sxs-lookup"><span data-stu-id="f06b6-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="f06b6-106">Чтобы узнать больше, узнайте, как настроить единый вход для [приложения-прокси приложения.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="f06b6-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="f06b6-107">Эта [статья используется для](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) устранения распространенных проблем, с которых сталкиваются люди при создании нового прокси-приложения приложения.</span><span class="sxs-lookup"><span data-stu-id="f06b6-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="f06b6-108">При проблеме настройки серверной проверки подлинности в приложении может потребоваться устранить неполадки конфигураций ограниченного делегирования [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) для прокси-сервера приложения или следовать указаниям по настройке приложения с [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) для решения проблемы.</span><span class="sxs-lookup"><span data-stu-id="f06b6-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
