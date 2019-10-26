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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747761"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Отказано в доступе при просмотре рабочего процесса

Рабочие процессы SharePoint 2013, которые пытаются отправить сообщение в группу SharePoint, могут привести к сбою с сообщением об ошибке "отказано в доступе", если для группы SharePoint не задано значение "все".
  
 **Чтобы устранить эту проблему, выполните указанные ниже действия.**
  
 1. Разрешить всем пользователям просматривать участников группы SharePoint.
  
 2. Удаление группы SharePoint из строки "Кому" или "копия" сообщения электронной почты.
  
 3. Явно добавьте пользователей в строку "Кому" или "копия", если невозможно изменить видимость членства для группы SharePoint.
  
Чтобы просмотреть дополнительные сведения, обратитесь к разделу [http несанкционированный доступ к/_vti_bin/Client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  