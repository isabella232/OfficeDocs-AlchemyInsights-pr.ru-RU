---
title: Изменение требований к надежному паролю
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706574"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="977a3-102">Изменение требований к надежному паролю</span><span class="sxs-lookup"><span data-stu-id="977a3-102">Change strong password requirement</span></span>

<span data-ttu-id="977a3-103">По умолчанию Майкрософт требует использования надежных паролей.</span><span class="sxs-lookup"><span data-stu-id="977a3-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="977a3-104">С помощью PowerShell можно отключить надежные пароли для определенных пользователей с помощью этой команды:</span><span class="sxs-lookup"><span data-stu-id="977a3-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="977a3-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – стронгпассвордрекуиред $false*</span><span class="sxs-lookup"><span data-stu-id="977a3-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="977a3-106">Дополнительные сведения о политике паролей</span><span class="sxs-lookup"><span data-stu-id="977a3-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="977a3-107">Подключение к Microsoft 365 с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="977a3-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="977a3-108">Дополнительные сведения о командах MsolUser PowerShell</span><span class="sxs-lookup"><span data-stu-id="977a3-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
