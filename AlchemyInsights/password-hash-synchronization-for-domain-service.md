---
title: Синхронизация хэша паролей для службы домена
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162941"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Синхронизация хэша паролей для службы домена

**Если ваш экземпляр Azure AD DS предлагает вам включить синхронизацию хэша паролей**

Это сценарий, в котором вы запускаете гибридную среду с пользователями, выполняя синхронизацию из локальной среды доменных служб Azure Active Directory (AD DS). Этот сценарий выполняется несмотря на синхронизацию хэша паролей из локальной службы AD DS с клиентом Azure AD.

**Причина**

Azure AD Connect по умолчанию не синхронизирует хэши паролей NTLM и Kerberos прежних версий, необходимые для Azure AD DS.

**Временное решение** 

Вам нужно настроить в Azure AD Connect синхронизацию хэшей паролей, необходимых для проверки подлинности NTLM и Kerberos.

После настройки Azure AD Connect во время локального события создания учетной записи или изменения пароля хэши паролей прежних версий также будут синхронизироваться с Azure AD. Дополнительные сведения об этом и рекомендации по включению синхронизации паролей в гибридных средах Azure AD DS см. [здесь](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).