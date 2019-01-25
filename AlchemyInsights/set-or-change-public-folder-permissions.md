---
title: Настройка или изменение разрешений для общей папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d537f1446318f1507f52297e547789fdf246b322
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500655"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="60e51-102">Разрешения и общих папок</span><span class="sxs-lookup"><span data-stu-id="60e51-102">Permissions and Public Folders</span></span>

<span data-ttu-id="60e51-103">Можно изменить разрешения на ваших общедоступных папок с помощью Outlook, Центр администрирования Exchange (EAC) или PowerShell:</span><span class="sxs-lookup"><span data-stu-id="60e51-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="60e51-104">Для получения инструкций Outlook, [щелкните здесь](https://support.office.com/article/https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="60e51-104">For Outlook instructions, [click here](https://support.office.com/article/https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="60e51-p101">Центр администрирования Exchange можно найти [в этой статье](https://support.office.com/article/https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) для получения инструкций. Щелкните [здесь](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) для перейдите в центр администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="60e51-p101">For EAC, refer to [this article](https://support.office.com/article/https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="60e51-p102">Powershell можно найти [в этой статье](https://support.office.com/article/https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) для получения инструкций по с помощью командлетов для Add-PublicFolderClientPermission. Если вам требуется инструкциям, чтобы подключиться к Exchange Powershell, щелкните [здесь](https://support.office.com/article/https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="60e51-p102">For Powershell, refer to [this article](https://support.office.com/article/https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://support.office.com/article/https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="60e51-p103">Если **внешние пользователи не могут отправлять сообщения электронной почты для общей папки с включенной поддержкой почты**, причина может быть что общей папки отсутствуют разрешения необходимо для доставки электронной почты внешним. Это можно устранить с помощью инструкции Outlook [здесь](https://support.office.com/article/https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)или инструкции PowerShell [здесь](https://support.office.com/article/https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="60e51-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://support.office.com/article/https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.office.com/article/https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

