---
title: Срок действия сертификата Федерации служб ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710420"
---
# <a name="adfs-federation-certificate-expiring"></a>Срок действия сертификата Федерации служб ADFS

Чтобы устранить эту проблему, выполните указанные ниже действия.
  
1. Установите модуль Microsoft Azure Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите в раздел [Manage Azure AD с помощью Windows PowerShell](https://aka.ms/aadposh).

2. Выполните действия, описанные в разделе "сценарий 1: срок действия сертификата подписи маркера AD FS истек" в разделе ["ошибка при доступе к сайту" из AD FS при входе федеративного пользователя в Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Выполните действия, описанные в [статье обновление или восстановление параметров федеративного домена в Microsoft, Azure или Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Дополнительные сведения об обновлении сертификатов федерации приведены в [статье обновление сертификатов федерации для Microsoft 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
