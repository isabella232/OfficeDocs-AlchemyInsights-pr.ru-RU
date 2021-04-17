---
title: Управление доступом к общедоступным папкам с помощью Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816753"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="e8b76-102">Управление доступом к общедоступным папкам с помощью Outlook</span><span class="sxs-lookup"><span data-stu-id="e8b76-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="e8b76-103">Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e8b76-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="e8b76-104">Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="e8b76-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="e8b76-105">$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook</span><span class="sxs-lookup"><span data-stu-id="e8b76-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="e8b76-106">$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook.</span><span class="sxs-lookup"><span data-stu-id="e8b76-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e8b76-107">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e8b76-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="e8b76-108">Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows.</span><span class="sxs-lookup"><span data-stu-id="e8b76-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e8b76-109">Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="e8b76-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="e8b76-110">Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="e8b76-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
