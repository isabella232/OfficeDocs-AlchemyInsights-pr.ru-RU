---
title: Управление доступом к общедоступным папкам с помощью Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680489"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="f8fa5-102">Управление доступом к общедоступным папкам с помощью Outlook</span><span class="sxs-lookup"><span data-stu-id="f8fa5-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="f8fa5-103">Чтобы указать, какие пользователи могут получать доступ к общедоступным папкам с помощью Outlook, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="f8fa5-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="f8fa5-104">Воспользуйтесь `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="f8fa5-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="f8fa5-105">$true: Разрешить пользователям получать доступ к общедоступным папкам в Outlook</span><span class="sxs-lookup"><span data-stu-id="f8fa5-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="f8fa5-106">$false. Запретить пользователям получать доступ к общедоступным папкам в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f8fa5-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="f8fa5-107">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8fa5-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="f8fa5-108">Примечание. Эта процедура может управлять подключениями только для клиентов с классической версией Outlook для Windows.</span><span class="sxs-lookup"><span data-stu-id="f8fa5-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="f8fa5-109">Пользователи могут по-прежнему получать доступ к общедоступным папкам с помощью веб-приложения Outlook или Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="f8fa5-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="f8fa5-110">Дополнительные сведения см. в статье [Управляемые подключения к общедоступным папкам в Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="f8fa5-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
