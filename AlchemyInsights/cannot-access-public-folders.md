---
title: Не удается получить доступ к общедоступным папкам
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341416"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="90057-102">Outlook не удается подключиться к общедоступным папкам</span><span class="sxs-lookup"><span data-stu-id="90057-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="90057-103">Если доступ к общедоступным папкам не работает для некоторых пользователей, попробуйте выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="90057-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="90057-104">Подключитесь к EXO PowerShell и настройте параметр DefaultPublicFolderMailbox учетной записи пользователя, чтобы он был сопоставлен с параметром рабочей учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="90057-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="90057-105">Пример.</span><span class="sxs-lookup"><span data-stu-id="90057-105">Example:</span></span>

<span data-ttu-id="90057-106">Get/Mailbox Воркингусер | ft DefaultPublicFolderMailbox, Еффективепубликфолдермаилбокс</span><span class="sxs-lookup"><span data-stu-id="90057-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="90057-107">Set — Mailbox Проблемусер — DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="90057-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="90057-108">Чтобы изменения вступили в силу, подождите хотя бы один час.</span><span class="sxs-lookup"><span data-stu-id="90057-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="90057-109">Если проблема не устранена, выполните указанные ниже [действия](https://aka.ms/pfcte) , чтобы устранить проблемы с доступом к общим папкам с помощью Outlook.</span><span class="sxs-lookup"><span data-stu-id="90057-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="90057-110">**Чтобы определить, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook**:</span><span class="sxs-lookup"><span data-stu-id="90057-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="90057-111">Используйте Set – CASMailbox <mailboxname> публикфолдерклиентакцесс $true или $false</span><span class="sxs-lookup"><span data-stu-id="90057-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="90057-112">$true: разрешить пользователям доступ к общедоступным папкам в Outlook</span><span class="sxs-lookup"><span data-stu-id="90057-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="90057-113">$false: запретить пользователям доступ к общедоступным папкам в Outlook.</span><span class="sxs-lookup"><span data-stu-id="90057-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="90057-114">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="90057-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="90057-115">Set — OrganizationConfig — Публикфолдершовклиентконтрол $true</span><span class="sxs-lookup"><span data-stu-id="90057-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="90057-116">**Note (Примечание** ) Эта процедура позволяет управлять подключениями только с клиентами Outlook Desktop для Windows.</span><span class="sxs-lookup"><span data-stu-id="90057-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="90057-117">Пользователь может продолжить доступ к общедоступным папкам с помощью OWA или Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="90057-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="90057-118">Дополнительные сведения приведены в статье [объявления о поддержке управляемых подключений для общедоступных папок в Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="90057-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>