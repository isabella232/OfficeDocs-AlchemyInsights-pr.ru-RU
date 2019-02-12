---
title: Службы федерации Active Directory Federation истечение срока действия сертификата
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925393"
---
# <a name="adfs-federation-certificate-expiring"></a>Службы федерации Active Directory Federation истечение срока действия сертификата

Чтобы устранить эту проблему, выполните следующие действия:
  
1. Установка Microsoft Azure модуль Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите на [Управление Azure AD, с помощью Windows PowerShell](https://aka.ms/aadposh).
    
2. Выполните действия, описанные в «сценарий 1: истек срок действия сертификата подписи маркера службы федерации Active Directory» раздела [«Возникла проблема, доступ к сайту»](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)ошибки из служб AD FS при входе федеративного пользователя в Office 365, Azure, или Intune.
    
3. Выполните действия, описанные в [том, как обновить или восстановить параметры федеративного домена в Office 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Дополнительные сведения об обновлении сертификатов федерации см [федерации Office 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

