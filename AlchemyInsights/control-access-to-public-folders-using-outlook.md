---
title: Управление доступом к общедоступным папкам с помощью Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406601"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="e210b-102">Управление доступом к общедоступным папкам с помощью Outlook</span><span class="sxs-lookup"><span data-stu-id="e210b-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="e210b-103">Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="e210b-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="e210b-104">Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="e210b-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="e210b-105">$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook</span><span class="sxs-lookup"><span data-stu-id="e210b-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="e210b-106">$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook.</span><span class="sxs-lookup"><span data-stu-id="e210b-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e210b-107">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e210b-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="e210b-108">Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows.</span><span class="sxs-lookup"><span data-stu-id="e210b-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e210b-109">Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="e210b-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="e210b-110">Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="e210b-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
