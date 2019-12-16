---
title: Начало работы с SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051654"
---
# <a name="workflows-in-sharepoint"></a>Рабочие процессы в SharePoint

Если рабочие процессы SharePoint не отправляют сообщения электронной почты, возможно, ваша организация обнаружила пределы отправителя Exchange Online.

Сообщение об ошибке "Рабочий процесс приостановлен" может появиться, если у вас есть один из следующих элементов:

- В SharePoint Online есть рабочий процесс, в котором используется тип платформы рабочих процессов SharePoint 2010 или SharePoint 2013.

- Рабочий процесс настроен на отправку настраиваемого сообщения электронной почты более чем 200 пользователям одновременно, более чем 10 000 получателей в день или более 30 сообщений в минуту.

При запуске рабочего процесса сообщение об ошибке не отправляется и отображается сообщение об ошибке, для параметра внутренний статус — "приостановлено" или "не удается отправить получателю".

Для получения дополнительных сведений обратитесь к следующей [статье](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

