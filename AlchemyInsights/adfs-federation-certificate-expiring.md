---
title: Срок действия сертификата федерации ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952982"
---
# <a name="adfs-federation-certificate-expiring"></a>Срок действия сертификата федерации ADFS

Чтобы устранить эту проблему, выполните следующие действия:
  
1. Установите модуль Microsoft Azure Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите к [управлению Azure AD с помощью Windows PowerShell.](https://aka.ms/aadposh)

2. Выполните действия в разделе "Сценарий 1: истек срок действия сертификата подписи маркеров AD FS" в разделе "Возникла проблема с доступом к сайту" ошибки [AD FS,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)когда федерарная пользователь войдет в Microsoft 365, Azure или Intune .

3. Выполните действия в обновлении или восстановлении параметров федерарного домена [в Microsoft, Azure или Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Дополнительные новости о возобновлении сертификатов Федерации см. в справке Об обновлении сертификатов федерации для Microsoft 365 [и Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
