---
title: Срок действия сертификата Федерации служб ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499904"
---
# <a name="adfs-federation-certificate-expiring"></a>Срок действия сертификата Федерации служб ADFS

Чтобы устранить эту проблему, выполните указанные ниже действия.
  
1. Установите модуль Microsoft Azure Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите в раздел [Manage Azure AD с помощью Windows PowerShell](https://aka.ms/aadposh).

2. Выполните действия, описанные в разделе "сценарий 1: срок действия сертификата подписи маркера AD FS истек" в разделе ["ошибка при доступе к сайту" из AD FS при входе федеративного пользователя в Office 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Выполните действия, описанные в статье [как обновить или восстановить параметры федеративного домена в Office 365, Azure или Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Дополнительные сведения об обновлении сертификатов федерации приведены в статье [Обновление сертификатов федерации для Office 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
