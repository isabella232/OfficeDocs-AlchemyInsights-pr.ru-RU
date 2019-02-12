---
title: 932 AADConnect обновление
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937957"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="14a95-102">Подключение обновления Azure AD</span><span class="sxs-lookup"><span data-stu-id="14a95-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="14a95-p101">По умолчанию автоматического обновления включена для Azure AD подключение, которое помогает, чтобы убедиться, что трассировка запускается последней версии. Чтобы проверить параметры автоматической обновления, используйте командлет **Get-ADSyncAutoUpgrade** в Windows Azure AD PowerShell. Командлет возвращает один из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="14a95-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="14a95-106">**Enabled**: включено автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="14a95-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="14a95-107">**Этот параметр отключен**: отключено автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="14a95-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="14a95-p102">**Приостановлено**: система больше не получают автоматического обновления. Нельзя настроить данное значение; оно установлено в системе.</span><span class="sxs-lookup"><span data-stu-id="14a95-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="14a95-110">Для получения дополнительных сведений см. [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="14a95-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="14a95-111">Чтобы загрузить последнюю версию Azure AD подключение, перейдите к [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="14a95-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

