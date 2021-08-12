---
title: Устранение неполадок с гостевых пользователей
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939392"
---
# <a name="troubleshoot-guest-user-issues"></a>Устранение неполадок с гостевых пользователей

1. Инструкции по управлению гостевым доступом к приложениям см. в руководстве по управлению гостевым доступом с помощью обзоров доступа [к Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Добавьте гостевых пользователей в каталог на [портале Azure.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)В этом quickstart вы добавите нового гостевого пользователя в каталог Azure AD через портал Azure, отправьте приглашение и посмотрите, как выглядит процесс выкупа приглашений гостевых пользователей.
1. [Добавьте гостевого пользователя в PowerShell.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)В этом quickstart вы будете использовать команду New-AzureADMSInvitation, чтобы добавить одного гостя в клиента Azure.
1. Чтобы узнать, как назначать пользователей и группы корпоративным приложениям в Azure Active Directory (Azure AD), либо на портале Azure, либо с помощью PowerShell, см. в статью Управление назначением пользователей для приложения в [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-совместная работа работает с большинством приложений, которые интегрируются с Azure AD. В этой [статье](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)мы пройдите инструкции по настройке некоторых популярных приложений SaaS для использования в Azure AD B2B.
1. Как организация, использующая возможности совместной Azure Active Directory (Azure AD) B2B для приглашения гостевых пользователей из партнерских организаций в Azure AD, теперь вы можете предоставить этим пользователям B2B доступ к локальному приложениям. Эти локальное приложение может использовать проверку подлинности на основе SAML или интегрированную Windows проверку подлинности (IWA) с ограниченной делегированием Kerberos (KCD). Дополнительные сведения см. в [приложении Grant B2B users in Azure AD access to your on-premises applications.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Узнайте, как предоставить учетным записям партнеров с локальным управлением доступ к облачным ресурсам с помощью совместной работы [Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)