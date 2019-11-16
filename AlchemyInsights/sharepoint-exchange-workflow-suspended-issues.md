---
title: Начало работы с SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766904"
---
# <a name="workflows-in-sharepoint"></a>Рабочие процессы в SharePoint

Если рабочие процессы SharePoint не отправляют сообщения электронной почты, возможно, ваша организация обнаружила пределы отправителя Exchange Online.

Сообщение об ошибке "Рабочий процесс приостановлен" может появиться, если у вас есть один из следующих элементов:

- В SharePoint Online есть рабочий процесс, в котором используется тип платформы рабочих процессов SharePoint 2010 или SharePoint 2013.

- Рабочий процесс настроен на отправку настраиваемого сообщения электронной почты более чем 200 пользователям одновременно, более чем 10 000 получателей в день или более 30 сообщений в минуту.

При запуске рабочего процесса сообщение об ошибке не отправляется и отображается сообщение об ошибке, для параметра внутренний статус — "приостановлено" или "не удается отправить получателю".

Для получения дополнительных сведений обратитесь к следующей [статье](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

