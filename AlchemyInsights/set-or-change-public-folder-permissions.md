---
title: Установка или изменение разрешений для общедоступных папок
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36734682"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="cf124-102">Разрешения и общедоступные папки</span><span class="sxs-lookup"><span data-stu-id="cf124-102">Permissions and Public Folders</span></span>

<span data-ttu-id="cf124-103">Вы можете изменить разрешения для общедоступных папок, используя Outlook, центр администрирования Exchange или PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cf124-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="cf124-104">Для получения инструкций для Outlook [щелкните здесь](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="cf124-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="cf124-105">За инструкциями центра администрирования Exchange обратитесь к [этой статье](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) .</span><span class="sxs-lookup"><span data-stu-id="cf124-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="cf124-106">В [этой статье](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) приведены инструкции по использованию командлета Add – PublicFolderClientPermission sharepointsync.</span><span class="sxs-lookup"><span data-stu-id="cf124-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="cf124-107">Если вам понадобятся инструкции по подключению к Exchange PowerShell, щелкните [здесь](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="cf124-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="cf124-108">Если **внешние пользователи не могут отправлять сообщения в общедоступную папку с включенной поддержкой почты**, причиной может быть то, что в общедоступной папке отсутствуют разрешения, необходимые для доставки внешних сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cf124-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="cf124-109">Это можно исправить с [помощью инструкций Outlook или инструкций PowerShell](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1) [.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="cf124-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

