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
# <a name="configure-ldap"></a>Настройка LDAP

Чтобы настроить LDAP, сделайте следующее:

1. Проверьте состояние домена на [портале Azure.](https://aka.ms/aadds-health)
1. Убедитесь, что доступна действительная подписка на Azure AD и включены доменные службы Azure AD.
1. Сертификат, необходимый для обеспечения безопасности LDAP, должен быть получен из доверенного публичного органа сертификации или быть самозаверяонным сертификатом.
1. Убедитесь, что сертификат следует [рекомендациям.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Недопустимый сертификат**
1. Чтобы обновить сертификат, выполните действия по созданию нового сертификата и повторной загрузке: [настройка LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Чтобы устранить известные проблемы с безопасными оповещениями LDAP в доменных службах Azure Active directory, см. "Устранение оповещений [LDAP".](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
