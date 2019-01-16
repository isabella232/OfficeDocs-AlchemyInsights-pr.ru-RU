---
title: Службы федерации Active Directory Federation истечение срока действия сертификата
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308335"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="c7f59-102">Службы федерации Active Directory Federation истечение срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="c7f59-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="c7f59-103">Чтобы устранить эту проблему, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="c7f59-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="c7f59-p101">Установка Microsoft Azure модуль Active Directory для Windows PowerShell на компьютере (если модуль еще не установлен). Для этого перейдите на [Управление Azure AD, с помощью Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="c7f59-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="c7f59-106">Выполните действия, описанные в «сценарий 1: истек срок действия сертификата подписи маркера службы федерации Active Directory» раздела [«Возникла проблема, доступ к сайту»](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)ошибки из служб AD FS при входе федеративного пользователя в Office 365, Azure, или Intune.</span><span class="sxs-lookup"><span data-stu-id="c7f59-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="c7f59-107">Выполните действия, описанные в [том, как обновить или восстановить параметры федеративного домена в Office 365, Azure или Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="c7f59-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="c7f59-108">Дополнительные сведения об обновлении сертификатов федерации см [федерации Office 365 и Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="c7f59-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

