---
title: Отказ в доступе при просмотре рабочего процесса
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955214"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Отказ в доступе при просмотре рабочего процесса

SharePoint 2013 г., которые пытаются отправить сообщение электронной почты в группу SharePoint, могут привести к сбой с сообщением об ошибке "Отказано в доступе", если членство SharePoint группы не установлено для всех.
  
 **Чтобы устранить эту проблему, сделайте следующие действия:**
  
 1. Разрешить всем видеть членов SharePoint группы.
  
 2. Удалите SharePoint группы из строки To или CC электронной почты.
  
 3. Явно добавьте пользователей в строку To или CC, если видимость членства не может быть изменена для SharePoint группы.
  
Дополнительные сведения см. в [http://http unauthorized to/_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  