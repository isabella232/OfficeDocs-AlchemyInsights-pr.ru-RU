---
title: Не отправляется сообщение электронной почты для рабочих процессов
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766146"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="7b119-102">Не отправляется сообщение электронной почты для списка или библиотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="7b119-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="7b119-103">Сообщения электронной почты от рабочих процессов не отправляются всем пользователям или только определенным пользователям или отображается сообщение об ошибке **: сообщение не может быть отправлено. Убедитесь, что в сообщении электронной почты есть действительный получатель**.</span><span class="sxs-lookup"><span data-stu-id="7b119-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="7b119-104">Проверьте, существует ли пользователь в группе разрешений " **все пользователи** " (список сведений о пользователях) для этого семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="7b119-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="7b119-105">URL-адрес прямого примера<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/People.aspx? Мембершипграупид = 0</span><span class="sxs-lookup"><span data-stu-id="7b119-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="7b119-106">Если пользователь не существует, убедитесь, что пользователь вошел на страницу.</span><span class="sxs-lookup"><span data-stu-id="7b119-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="7b119-107">Если это внешний пользователь, убедитесь, что его приглашение принято.</span><span class="sxs-lookup"><span data-stu-id="7b119-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="7b119-108">Если пользователь существует в группе разрешений, убедитесь, что адрес электронной почты задан правильно.</span><span class="sxs-lookup"><span data-stu-id="7b119-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="7b119-109">Если адрес электронной почты пользователя не задан, создайте пример оповещения для этого пользователя, который принудительно выполняет синхронизацию учетной записи этого пользователя с профилями пользователей SharePoint с этим семейством веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="7b119-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="7b119-110">Сообщения электронной почты от рабочих процессов отправляются администраторам семейства веб-сайтов, но не отправляются другим пользователям и отображаются ошибки **http, запрещенные для <span>https:</span>//УРЛ/_vti_bin/клиент.КСВК.СП.утилитиес.утилити.сендемаил**.</span><span class="sxs-lookup"><span data-stu-id="7b119-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="7b119-111">[В статье отказ в доступе при отправке сообщения электронной почты в группу SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="7b119-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="7b119-112">Кроме того, убедитесь, что компонент "семейство веб-сайтов **с ограниченным доступом" не активен в режиме ограниченного доступа** .</span><span class="sxs-lookup"><span data-stu-id="7b119-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="7b119-113">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="7b119-113">Related topics</span></span>
<span data-ttu-id="7b119-114">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="7b119-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7b119-115">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="7b119-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7b119-116">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="7b119-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


