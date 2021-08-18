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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090425"
---
# <a name="configure-ldap"></a>Настройка LDAP

Чтобы настроить LDAP, сделайте следующее:

1. Проверьте состояние домена на портале [Azure.](https://aka.ms/aadds-health)
1. Убедитесь, что доступна действительная подписка Azure AD и включены службы домена Azure AD.
1. Сертификат, необходимый для обеспечения безопасности LDAP, должен быть получен из доверенного органа государственной сертификации или иметь самозаверяемый сертификат.
1. Убедитесь, что сертификат следует требуемой [инструкции.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Недействительный сертификат**
1. Чтобы обновить сертификат, выполните действия по созданию нового сертификата и повторной загрузке: [Настройка LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Чтобы устранить известные проблемы с помощью безопасных оповещений LDAP в службах домена Azure Active directory, см. в [рублях Resolve LDAP alerts.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
