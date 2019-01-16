---
title: Включение аудита почтовых ящиков
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307895"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="09c5c-102">Включение аудита почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="09c5c-102">Enable mailbox auditing</span></span>

<span data-ttu-id="09c5c-103">Для включения аудита почтовых ящиков для одного пользователя или всей организации необходимо выполнить следующие командлеты из удаленной оболочки питания:</span><span class="sxs-lookup"><span data-stu-id="09c5c-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="09c5c-104">**Одного пользователя**</span><span class="sxs-lookup"><span data-stu-id="09c5c-104">**Single User**</span></span>
  
<span data-ttu-id="09c5c-105">Set-Mailbox - Identity «Jane Dow» - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="09c5c-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="09c5c-106">**Организация**</span><span class="sxs-lookup"><span data-stu-id="09c5c-106">**Organization**</span></span>
  
<span data-ttu-id="09c5c-107">Get-Mailbox - ResultSize неограниченное - фильтрации {RecipientTypeDetails - eq «UserMailbox»} | Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="09c5c-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="09c5c-108">Подробнее</span><span class="sxs-lookup"><span data-stu-id="09c5c-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

