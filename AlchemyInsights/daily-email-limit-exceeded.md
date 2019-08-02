---
title: Превышен ежедневный лимит электронной почты. Рабочий процесс приостановлен.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059651"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="271e5-103">Превышен ежедневный лимит электронной почты.</span><span class="sxs-lookup"><span data-stu-id="271e5-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="271e5-104">Рабочий процесс приостановлен.</span><span class="sxs-lookup"><span data-stu-id="271e5-104">Workflow is suspended.</span></span>

<span data-ttu-id="271e5-105">Эту ошибку можно получить в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="271e5-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="271e5-106">В SharePoint Online есть рабочий процесс, в котором используется тип платформы рабочих процессов SharePoint 2010 или SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="271e5-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="271e5-107">Рабочий процесс настроен на отправку настраиваемого сообщения электронной почты более чем 200 пользователям одновременно, более чем 10 000 получателей в день или более 30 сообщений в минуту.</span><span class="sxs-lookup"><span data-stu-id="271e5-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="271e5-108">При запуске рабочего процесса сообщение электронной почты не отправляется и обратите внимание на следующее поведение:</span><span class="sxs-lookup"><span data-stu-id="271e5-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="271e5-109">Для рабочего процесса, использующего тип платформы SharePoint 2013, перейдите на страницу **состояния рабочего процесса** .</span><span class="sxs-lookup"><span data-stu-id="271e5-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="271e5-110">На странице "состояние рабочего процесса" для параметра **внутренний статус** задано значение **начато**, а всплывающая подсказка **не может быть отправлена получателю**.</span><span class="sxs-lookup"><span data-stu-id="271e5-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="271e5-111">Чтобы обойти эту проблему, настройте рабочий процесс на отправку сообщений электронной почты без превышения ограничения на количество отправителей в [Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="271e5-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="271e5-112">Например, используйте паузу в рабочем процессе, отправьте сообщение электронной почты в группу Office 365, группу рассылки или группу безопасности с включенной поддержкой почты или отправьте сообщение менее чем 200 получателям одновременно.</span><span class="sxs-lookup"><span data-stu-id="271e5-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="271e5-113">Более подробную информацию можно найти в следующей [статье](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="271e5-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="271e5-114">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="271e5-114">Related topics</span></span>
- [<span data-ttu-id="271e5-115">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="271e5-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="271e5-116">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="271e5-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 