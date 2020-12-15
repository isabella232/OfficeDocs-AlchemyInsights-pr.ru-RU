---
title: Изменение адреса электронной почты группы Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416702"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="e369e-102">Изменение адреса электронной почты группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e369e-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="e369e-103">Вы можете изменить адрес электронной почты группы Microsoft 365, используя Центр администрирования.</span><span class="sxs-lookup"><span data-stu-id="e369e-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="e369e-104">Достаточно выбрать группу, а затем выбрать @Изменить адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e369e-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="e369e-105">Также можно использовать следующую команду EXO PowerShell, чтобы изменить основной SMTP-адрес группы Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="e369e-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="e369e-106">Пример:</span><span class="sxs-lookup"><span data-stu-id="e369e-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
