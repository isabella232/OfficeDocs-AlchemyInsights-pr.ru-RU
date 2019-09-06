---
title: Отказано в доступе при просмотре рабочего процесса
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747761"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="f246b-102">Отказано в доступе при просмотре рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="f246b-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="f246b-103">Рабочие процессы SharePoint 2013, которые пытаются отправить сообщение в группу SharePoint, могут привести к сбою с сообщением об ошибке "отказано в доступе", если для группы SharePoint не задано значение "все".</span><span class="sxs-lookup"><span data-stu-id="f246b-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="f246b-104">**Чтобы устранить эту проблему, выполните указанные ниже действия.**</span><span class="sxs-lookup"><span data-stu-id="f246b-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="f246b-105">Разрешить всем пользователям просматривать участников группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f246b-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="f246b-106">Удаление группы SharePoint из строки "Кому" или "копия" сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f246b-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="f246b-107">Явно добавьте пользователей в строку "Кому" или "копия", если невозможно изменить видимость членства для группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f246b-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="f246b-108">Чтобы просмотреть дополнительные сведения, обратитесь к разделу [http несанкционированный доступ к/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f246b-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  