---
title: Отказано в доступе при просмотре рабочего процесса
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883604"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e7560-102">Отказано в доступе при просмотре рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="e7560-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e7560-103">Рабочие процессы SharePoint 2013, которые пытаются отправить сообщение в группу SharePoint, могут привести к сбою с сообщением об ошибке "отказано в доступе", если для группы SharePoint не задано значение "все".</span><span class="sxs-lookup"><span data-stu-id="e7560-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e7560-104">**Чтобы устранить эту проблему, выполните указанные ниже действия.**</span><span class="sxs-lookup"><span data-stu-id="e7560-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e7560-105">Разрешить всем пользователям просматривать участников группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e7560-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e7560-106">Удаление группы SharePoint из строки "Кому" или "копия" сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e7560-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e7560-107">Явно добавьте пользователей в строку "Кому" или "копия", если невозможно изменить видимость членства для группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e7560-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e7560-108">Чтобы просмотреть дополнительные сведения, обратитесь к разделу HTTP несанкционированный доступ [к/_вти_бин/клиент.СВК/СП.утилитиес.утилити.сендемаил](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="e7560-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  