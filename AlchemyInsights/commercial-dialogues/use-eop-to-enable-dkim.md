---
title: Используйте Exchange Online PowerShell, чтобы включить DKIM для определенного домена
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737654"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="92c46-102">Используйте Exchange Online PowerShell, чтобы включить DKIM для определенного домена</span><span class="sxs-lookup"><span data-stu-id="92c46-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="92c46-103">Если вы не можете создать записи DKIM DNS в центре администрирования, попробуйте использовать Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="92c46-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="92c46-104">Чтобы создать DKIM-запись DNS с помощью Exchange Online PowerShell, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="92c46-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="92c46-105">Откройте Windows PowerShell администратора и запустите следующие команды в описанной последовательности:</span><span class="sxs-lookup"><span data-stu-id="92c46-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="92c46-106">а.</span><span class="sxs-lookup"><span data-stu-id="92c46-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="92c46-107">b.</span><span class="sxs-lookup"><span data-stu-id="92c46-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="92c46-108">в.</span><span class="sxs-lookup"><span data-stu-id="92c46-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="92c46-109">Если у вас возникли проблемы с подключением к Exchange Online PowerShell, см. в обзоре [Connect to Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="92c46-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="92c46-110">После подключения к Exchange Online PowerShell запустите следующую команду:</span><span class="sxs-lookup"><span data-stu-id="92c46-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="92c46-111">После успешного выполнения вышеуказанной команды запустите следующую команду, чтобы завершить сеанс PowerShell Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="92c46-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



