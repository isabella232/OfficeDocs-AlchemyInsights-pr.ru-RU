---
title: Срок действия одного из локальных сертификатов службы федерации истечет
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419705"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Срок действия одного из локальных сертификатов службы федерации истечет

Чтобы устранить эту проблему, выполните указанные ниже действия.
  
- Установите модуль Microsoft Azure Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите в [Azure Active Directory PowerShell для Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Выполните действия, описанные в разделе "сценарий 1: срок действия сертификата подписи маркера AD FS истек" в разделе ["ошибка при доступе к сайту" из AD FS при входе федеративного пользователя в Office 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Выполните действия, описанные в статье[как обновление или восстановление параметров федеративного домена в Office 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Дополнительные сведения об обновлении сертификатов федерации приведены в статье [Обновление сертификатов для O365 и Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

