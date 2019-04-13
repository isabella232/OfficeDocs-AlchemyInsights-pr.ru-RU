---
title: 932 обновление AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858973"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="ca372-102">Обновление Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="ca372-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="ca372-103">По умолчанию автоматическое обновление включено для Azure AD Connect, что позволяет убедиться, что вы используете последнюю версию.</span><span class="sxs-lookup"><span data-stu-id="ca372-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="ca372-104">Чтобы проверить параметры автоматического обновления, используйте командлет **Get – адсинкаутаупграде** в Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ca372-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="ca372-105">Командлет возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="ca372-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="ca372-106">**Enabled**: автоматическое обновление включено.</span><span class="sxs-lookup"><span data-stu-id="ca372-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="ca372-107">**Disabled**: автоматическое обновление отключено.</span><span class="sxs-lookup"><span data-stu-id="ca372-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="ca372-108">**Suspended**: система больше не имеет права на получение автоматических обновлений.</span><span class="sxs-lookup"><span data-stu-id="ca372-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="ca372-109">Вы не можете настроить это значение; Он задается системой.</span><span class="sxs-lookup"><span data-stu-id="ca372-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="ca372-110">Более подробную информацию можно узнать в статье [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="ca372-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="ca372-111">Чтобы скачать последнюю версию Azure AD Connect, перейдите по [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)адресу.</span><span class="sxs-lookup"><span data-stu-id="ca372-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
