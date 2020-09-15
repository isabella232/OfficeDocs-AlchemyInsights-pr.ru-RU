---
title: Срок действия сертификата федерации ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686762"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="debc8-102">Срок действия сертификата федерации ADFS</span><span class="sxs-lookup"><span data-stu-id="debc8-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="debc8-103">Чтобы устранить эту проблему, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="debc8-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="debc8-104">Установите модуль Microsoft Azure Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен).</span><span class="sxs-lookup"><span data-stu-id="debc8-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="debc8-105">Для этого перейдите в раздел [Manage Azure AD с помощью Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="debc8-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="debc8-106">Выполните действия, описанные в разделе "сценарий 1: срок действия сертификата подписи маркера AD FS истек" в разделе ["ошибка при доступе к сайту" из AD FS при входе федеративного пользователя в Microsoft 365, Azure или Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="debc8-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="debc8-107">Выполните действия, описанные в [статье обновление или восстановление параметров федеративного домена в Microsoft, Azure или Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="debc8-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="debc8-108">Дополнительные сведения об обновлении сертификатов федерации приведены в [статье обновление сертификатов федерации для Microsoft 365 и Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="debc8-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
