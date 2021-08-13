---
title: Истек срок действия одного из локального сертификата служб Федерации
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985230"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Истек срок действия одного из локального сертификата служб Федерации

Чтобы устранить эту проблему, выполните следующие действия:
  
- Установите модуль Microsoft Azure Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите [в Azure Active Directory PowerShell для Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Выполните действия в разделе "Сценарий 1: истек срок действия сертификата подписи маркеров AD FS" в разделе "Возникла проблема с доступом к сайту" ошибки [AD FS,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)когда федерарная пользователь войдет в Microsoft 365, Azure или Intune .
    
- Выполните действия в области Обновления или восстановления параметров федератного домена в [Microsoft 365, Azure или Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Дополнительные сведения о возобновлении сертификатов Федерации см. в дополнительных сведениях о продлении сертификатов [для O365 и Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

