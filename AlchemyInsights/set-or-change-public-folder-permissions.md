---
title: Настройка или изменение разрешений общедоступных папок
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789220"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="af7cd-102">Разрешения и общедоступные папки</span><span class="sxs-lookup"><span data-stu-id="af7cd-102">Permissions and Public Folders</span></span>

<span data-ttu-id="af7cd-103">Разрешения в общедоступных папках можно изменить с помощью Outlook, центра администрирования Exchange (EAC) или PowerShell:</span><span class="sxs-lookup"><span data-stu-id="af7cd-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="af7cd-104">Инструкции Outlook нажмите [здесь](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="af7cd-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="af7cd-105">Для EAC обратитесь к [этой статье для](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) инструкций.</span><span class="sxs-lookup"><span data-stu-id="af7cd-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="af7cd-106">Для Powershell обратитесь к [этой статье](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) для инструкций по использованию командного Add-PublicFolderClientPermission.</span><span class="sxs-lookup"><span data-stu-id="af7cd-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="af7cd-107">Если вам нужны инструкции для подключения к Exchange Powershell, нажмите [здесь](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="af7cd-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="af7cd-108">Если **внешние** пользователи не могут отправлять электронные письма в общедоступные папки с включенной почтой, причина может быть в том, что в публичной папке отсутствуют разрешения, необходимые для внешней доставки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="af7cd-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="af7cd-109">Это можно исправить с помощью инструкций Outlook [здесь](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)или инструкций PowerShell [здесь](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="af7cd-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

