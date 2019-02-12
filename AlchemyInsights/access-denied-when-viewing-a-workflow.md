---
title: Доступ запрещен при просмотре рабочего процесса
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918841"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="b37bf-102">Доступ запрещен при просмотре рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="b37bf-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="b37bf-103">Рабочих процессов SharePoint 2013, при попытке отправить сообщение электронной почты в группу SharePoint может не работать с сообщением об ошибке «Отказано в доступе», если для членов группы SharePoint не задано для всех.</span><span class="sxs-lookup"><span data-stu-id="b37bf-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="b37bf-104">**Чтобы устранить эту проблему, выполните следующие действия:**</span><span class="sxs-lookup"><span data-stu-id="b37bf-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="b37bf-105">Разрешить всем пользователям просмотреть список членов группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b37bf-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="b37bf-106">Удаление группы SharePoint из «Кому» или «копия» строки сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b37bf-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="b37bf-107">Явным образом добавьте пользователей в поле Кому или копия строки, если членство видимости нельзя изменить для группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b37bf-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="b37bf-108">Для просмотра более подробных сведений обратитесь к [Несанкционированного HTTP для /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b37bf-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

