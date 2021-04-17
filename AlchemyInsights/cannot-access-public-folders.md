---
title: Невозможно получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819525"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="1ebfd-102">Outlook не может подключаться к общедоступным папкам</span><span class="sxs-lookup"><span data-stu-id="1ebfd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="1ebfd-103">Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="1ebfd-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="1ebfd-104">Подключись к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox в учетной записи пользователя проблемы, чтобы соответствовать параметру рабочей учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="1ebfd-105">Пример.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-105">Example:</span></span>

<span data-ttu-id="1ebfd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="1ebfd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="1ebfd-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="1ebfd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="1ebfd-108">Подождите по крайней мере один час, пока изменение вступает в силу.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="1ebfd-109">Если проблема сохраняется, выполните эту [процедуру,](https://aka.ms/pfcte) чтобы устранить проблемы с доступом к общедоступным папам с помощью Outlook.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="1ebfd-110">**Управление доступом пользователей к общедоступным папкам с помощью Outlook:**</span><span class="sxs-lookup"><span data-stu-id="1ebfd-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="1ebfd-111">Используйте <mailboxname> Set-CASMailbox-PublicFolderClientAccess $true или $false</span><span class="sxs-lookup"><span data-stu-id="1ebfd-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="1ebfd-112">$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook</span><span class="sxs-lookup"><span data-stu-id="1ebfd-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="1ebfd-113">$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="1ebfd-114">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="1ebfd-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="1ebfd-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="1ebfd-116">**Примечание** Эта процедура может управлять подключениями только с настольным компьютером Outlook для клиентов Windows.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="1ebfd-117">Пользователь может продолжить доступ к общедоступным папкам с помощью OWA или Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="1ebfd-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="1ebfd-118">Дополнительные сведения см. в анонсе "Поддержка контролируемых подключений к [общедоступным папкам в Outlook".](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="1ebfd-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>