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
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389900"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Отказано в доступе при просмотре рабочего процесса

Рабочие процессы SharePoint 2013, которые пытаются отправить сообщение в группу SharePoint, могут привести к сбою с сообщением об ошибке "отказано в доступе", если для группы SharePoint не задано значение "все".
  
 **Чтобы устранить эту проблему, выполните указанные ниже действия.**
  
 1. Разрешить всем пользователям просматривать участников группы SharePoint. 
  
 2. Удаление группы SharePoint из строки "Кому" или "копия" сообщения электронной почты. 
  
 3. Явно добавьте пользователей в строку "Кому" или "копия", если невозможно изменить видимость членства для группы SharePoint. 
  
Чтобы просмотреть дополнительные сведения, обратитесь к разделу HTTP неСанкционированный доступ [к/_вти_бин/клиент.СВК/СП.утилитиес.утилити.сендемаил ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

