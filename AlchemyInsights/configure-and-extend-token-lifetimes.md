---
title: Настройка и увеличение жизненного цикла маркеров
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912028"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="d6a38-102">Настройка и увеличение жизненного цикла маркеров</span><span class="sxs-lookup"><span data-stu-id="d6a38-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="d6a38-103">Вы можете указать жизненный цикл маркера доступа, SAML или идентификатора, выданного платформой удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d6a38-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="d6a38-104">Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="d6a38-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="d6a38-105">Дополнительные сведения см. в статье [Настраиваемые жизненные циклы маркера](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="d6a38-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="d6a38-106">Например, см. статью [Примеры настройки жизненного цикла маркеров](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="d6a38-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="d6a38-107">Сведения о настройке жизненного цикла и совместимости маркеров в Azure Active Directory B2C (Azure AD B2C), см. в статье [Настройка маркеров в Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="d6a38-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="d6a38-108">Статья [Настройка сеанса в службе Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) описывает методы единого входа (SSO), используемые в Azure AD B2C, и помогает выбрать подходящий способ единого входа при настройке политики.</span><span class="sxs-lookup"><span data-stu-id="d6a38-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="d6a38-109">**В течение какого времени действуют маркеры? В течение какого времени они действительны?**</span><span class="sxs-lookup"><span data-stu-id="d6a38-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="d6a38-110">Жизненный цикл маркеров составляет 1 час, а жизненный цикл сеанса — 24 часа.</span><span class="sxs-lookup"><span data-stu-id="d6a38-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="d6a38-111">Это означает, что если запросы не были выполнены в течение 24 часов, перед запросом нового маркера потребуется выполнить вход еще раз.</span><span class="sxs-lookup"><span data-stu-id="d6a38-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="d6a38-112">После 30 мая 2020 г. новый клиент не сможет использовать настраиваемую политику жизненных циклов маркеров для настройки сеанса и обновления маркеров.</span><span class="sxs-lookup"><span data-stu-id="d6a38-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="d6a38-113">Прекращение поддержки происходит в течение нескольких месяцев. Это означает, что мы не будем учитывать существующие политики сеанса и обновления маркеров.</span><span class="sxs-lookup"><span data-stu-id="d6a38-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="d6a38-114">Вы можете настроить жизненный цикл маркеров доступа после прекращение поддержки.</span><span class="sxs-lookup"><span data-stu-id="d6a38-114">You can still configure access token lifetimes after the deprecation.</span></span>






