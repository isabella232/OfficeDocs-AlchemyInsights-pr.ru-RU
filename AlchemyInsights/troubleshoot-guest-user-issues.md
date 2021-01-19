---
title: Устранение неполадок гостевых пользователей
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897749"
---
# <a name="troubleshoot-guest-user-issues"></a>Устранение неполадок гостевых пользователей

1. Руководство по управлению гостевым доступом к приложениям см. в руководстве "Управление гостевым доступом с помощью проверок доступа [Azure AD".](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Добавьте гостевых пользователей в каталог на портале [Azure.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)В этом кратком примере вы добавите нового гостевого пользователя в каталог Azure AD через портал Azure, отправьте приглашение и посмотрите, как выглядит процесс активации приглашения гостевого пользователя.
1. Добавьте гостевого пользователя с [помощью PowerShell.](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)В этом кратком New-AzureADMSInvitation вы добавите одного гостевого пользователя в клиент Azure.
1. Чтобы узнать, как назначать пользователей и группы корпоративным приложениям в Azure Active Directory (Azure AD) на портале Azure или с помощью PowerShell, см. статью "Управление назначением пользователей для приложения в [Azure Active Directory".](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Совместная работа B2B Azure Active Directory (Azure AD) работает с большинством приложений, которые интегрируются с Azure AD. В этой [статье](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)мы поимяем инструкции по настройке некоторых популярных приложений SaaS для использования с Azure AD B2B.
1. Как организация, использующая возможности совместной работы Azure Active Directory (Azure AD) B2B для приглашения гостевых пользователей из партнерских организаций в Azure AD, вы можете предоставить этим пользователям B2B доступ к локальному приложениям. Эти приложения могут использовать проверку подлинности на основе SAML или встроенную проверку подлинности Windows (IWA) с ограниченным делегированием Kerberos (KCD). Дополнительные сведения см. в подсети "Предоставление пользователям [B2B в Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)доступа к вашим приложениям в локальной сети".
1. Узнайте, как предоставить учетным записям партнеров, управляемым локально, доступ к облачным ресурсам с помощью совместной работы [Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)