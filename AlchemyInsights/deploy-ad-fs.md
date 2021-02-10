---
title: Развертывание AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50165271"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="33f98-102">Развертывание AD FS</span><span class="sxs-lookup"><span data-stu-id="33f98-102">Deploy AD FS</span></span>

<span data-ttu-id="33f98-103">Развертывание служб федерации Active Directory (AD FS) использует вашу локальной инфраструктуру для проверки подлинности пользователей для служб Office 365.</span><span class="sxs-lookup"><span data-stu-id="33f98-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="33f98-104">Благодаря федеративному входу вы можете позволить пользователям вошел в службы Office 365 и приложения SAAS, интегрированные с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="33f98-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="33f98-105">Федераированный вход позволяет проверить подлинность пользователей в локальной службе Active Directory с помощью AD FS.</span><span class="sxs-lookup"><span data-stu-id="33f98-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="33f98-106">Кроме того, в корпоративной сети пользователям не потребуется повторно вводить свои пароли.</span><span class="sxs-lookup"><span data-stu-id="33f98-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="33f98-107">Помощник по развертыванию [AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) предоставляет пошаговые инструкции по развертыванию локальной инфраструктуры AD FS, которая обеспечивает проверку подлинности пользователей для служб Microsoft 365 и Office 365.</span><span class="sxs-lookup"><span data-stu-id="33f98-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="33f98-108">С помощью этого руководства ваша организация может просмотреть компоненты и требования AD FS, приобрести и установить SSL-сертификаты, необходимые для развертывания, и установить необходимый прокси-сервер веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="33f98-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
