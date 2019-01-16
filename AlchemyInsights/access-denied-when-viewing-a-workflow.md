---
title: Доступ запрещен при просмотре рабочего процесса
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308144"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Доступ запрещен при просмотре рабочего процесса

Рабочих процессов SharePoint 2013, при попытке отправить сообщение электронной почты в группу SharePoint может не работать с сообщением об ошибке «Отказано в доступе», если для членов группы SharePoint не задано для всех.
  
 **Чтобы устранить эту проблему, выполните следующие действия:**
  
 1. Разрешить всем пользователям просмотреть список членов группы SharePoint. 
  
 2. Удаление группы SharePoint из «Кому» или «копия» строки сообщение электронной почты. 
  
 3. Явным образом добавьте пользователей в поле Кому или копия строки, если членство видимости нельзя изменить для группы SharePoint. 
  
Для просмотра более подробных сведений обратитесь к [Несанкционированного HTTP для /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

