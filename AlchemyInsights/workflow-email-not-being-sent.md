---
title: Не отправляется сообщение электронной почты для рабочих процессов
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
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270685"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="5c106-102">Не отправляется сообщение электронной почты для рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="5c106-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="5c106-103">Сообщения электронной почты от рабочих процессов не отправляются всем пользователям или только определенным пользователям или отображается сообщение об ошибке **: сообщение не может быть отправлено. Убедитесь, что в сообщении электронной почты есть действительный получатель**.</span><span class="sxs-lookup"><span data-stu-id="5c106-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="5c106-104">Проверьте, существует ли пользователь в группе разрешений " **все пользователи** " (список сведений о пользователях) для этого семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="5c106-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="5c106-105">Пример прямого URL-адреса<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/People.aspx? Мембершипграупид = 0</span><span class="sxs-lookup"><span data-stu-id="5c106-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="5c106-106">Если пользователь не существует, убедитесь, что пользователь вошел на страницу.</span><span class="sxs-lookup"><span data-stu-id="5c106-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="5c106-107">Если это внешний пользователь, убедитесь, что его приглашение принято.</span><span class="sxs-lookup"><span data-stu-id="5c106-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="5c106-108">Если пользователь существует в группе разрешений, убедитесь, что адрес электронной почты задан правильно.</span><span class="sxs-lookup"><span data-stu-id="5c106-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="5c106-109">Если адрес электронной почты пользователя не задан, создайте пример оповещения для этого пользователя, который принудительно выполняет синхронизацию учетной записи этого пользователя с профилями пользователей SharePoint с этим семейством веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="5c106-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="5c106-110">Сообщения электронной почты от рабочих процессов отправляются администраторам семейства веб-сайтов, но не другим пользователям, и просмотр ошибки \*\*http запрещен <spam> <spam>. \*\* <spam> <spam></span><span class="sxs-lookup"><span data-stu-id="5c106-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="5c106-111">[В статье отказ в доступе при отправке сообщения электронной почты группам](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="5c106-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="5c106-112">Кроме того, убедитесь, что компонент "семейство веб-сайтов с ограниченным доступом" не активен в **режиме ограниченного доступа** .</span><span class="sxs-lookup"><span data-stu-id="5c106-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="5c106-113">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="5c106-113">Related topics</span></span>
<span data-ttu-id="5c106-114">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="5c106-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5c106-115">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="5c106-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5c106-116">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="5c106-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


