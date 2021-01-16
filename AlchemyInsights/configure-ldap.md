---
title: Настройка LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876570"
---
# <a name="configure-ldap"></a><span data-ttu-id="288d8-102">Настройка LDAP</span><span class="sxs-lookup"><span data-stu-id="288d8-102">Configure LDAP</span></span>

<span data-ttu-id="288d8-103">Чтобы настроить LDAP, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="288d8-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="288d8-104">Проверьте состояние домена на [портале Azure.](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="288d8-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="288d8-105">Убедитесь, что доступна действительная подписка на Azure AD и включены доменные службы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="288d8-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="288d8-106">Сертификат, необходимый для обеспечения безопасности LDAP, должен быть получен из доверенного публичного органа сертификации или быть самозаверяонным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="288d8-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="288d8-107">Убедитесь, что сертификат следует [рекомендациям.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)</span><span class="sxs-lookup"><span data-stu-id="288d8-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="288d8-108">**Недопустимый сертификат**</span><span class="sxs-lookup"><span data-stu-id="288d8-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="288d8-109">Чтобы обновить сертификат, выполните действия по созданию нового сертификата и повторной загрузке: [настройка LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="288d8-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="288d8-110">Чтобы устранить известные проблемы с безопасными оповещениями LDAP в доменных службах Azure Active directory, см. "Устранение оповещений [LDAP".](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="288d8-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
