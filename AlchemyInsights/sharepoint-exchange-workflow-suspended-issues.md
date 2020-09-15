---
title: Начало работы с SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700720"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="f0efb-102">Рабочие процессы в SharePoint</span><span class="sxs-lookup"><span data-stu-id="f0efb-102">Workflows in SharePoint</span></span>

<span data-ttu-id="f0efb-103">Если рабочие процессы SharePoint не отправляют сообщения электронной почты, возможно, ваша организация обнаружила пределы отправителя Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f0efb-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="f0efb-104">Сообщение об ошибке "Рабочий процесс приостановлен" может появиться, если у вас есть один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="f0efb-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="f0efb-105">В SharePoint Online есть рабочий процесс, в котором используется тип платформы рабочих процессов SharePoint 2010 или SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="f0efb-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="f0efb-106">Рабочий процесс настроен на отправку настраиваемого сообщения электронной почты более чем 200 пользователям одновременно, более чем 10 000 получателей в день или более 30 сообщений в минуту.</span><span class="sxs-lookup"><span data-stu-id="f0efb-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="f0efb-107">При запуске рабочего процесса сообщение об ошибке не отправляется и отображается сообщение об ошибке, для параметра внутренний статус — "приостановлено" или "не удается отправить получателю".</span><span class="sxs-lookup"><span data-stu-id="f0efb-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="f0efb-108">Для получения дополнительных сведений обратитесь к следующей [статье](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="f0efb-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

