---
title: 932 обновление AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506096"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="7e115-102">Обновление Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="7e115-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="7e115-103">По умолчанию автоматическое обновление включено для Azure AD Connect, что позволяет убедиться, что вы используете последнюю версию.</span><span class="sxs-lookup"><span data-stu-id="7e115-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="7e115-104">Чтобы проверить параметры автоматического обновления, используйте командлет **Get – адсинкаутаупграде** в Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7e115-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="7e115-105">Командлет возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="7e115-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="7e115-106">**Enabled**: автоматическое обновление включено.</span><span class="sxs-lookup"><span data-stu-id="7e115-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="7e115-107">**Disabled**: автоматическое обновление отключено.</span><span class="sxs-lookup"><span data-stu-id="7e115-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="7e115-108">**Suspended**: система больше не имеет права на получение автоматических обновлений.</span><span class="sxs-lookup"><span data-stu-id="7e115-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="7e115-109">Вы не можете настроить это значение; Он задается системой.</span><span class="sxs-lookup"><span data-stu-id="7e115-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="7e115-110">Более подробную информацию можно узнать в статье [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="7e115-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="7e115-111">Чтобы скачать последнюю версию Azure AD Connect, перейдите по [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)адресу.</span><span class="sxs-lookup"><span data-stu-id="7e115-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
