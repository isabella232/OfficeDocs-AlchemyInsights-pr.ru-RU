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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733700"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="2af86-102">Изменение адреса электронной почты группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2af86-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="2af86-103">Вы можете изменить адрес электронной почты группы Microsoft 365, используя Центр администрирования.</span><span class="sxs-lookup"><span data-stu-id="2af86-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="2af86-104">Достаточно выбрать группу, а затем выбрать @Изменить адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2af86-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="2af86-105">Также можно использовать следующую команду EXO PowerShell, чтобы изменить основной SMTP-адрес группы Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="2af86-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="2af86-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="2af86-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="2af86-107">Пример:</span><span class="sxs-lookup"><span data-stu-id="2af86-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
