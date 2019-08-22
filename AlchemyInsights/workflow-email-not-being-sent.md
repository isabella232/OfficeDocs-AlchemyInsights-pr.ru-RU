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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530900"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="fa08b-102">Не отправляется сообщение электронной почты для списка или библиотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="fa08b-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="fa08b-103">Сообщения электронной почты от рабочих процессов не отправляются всем пользователям или только определенным пользователям или отображается сообщение об ошибке **: сообщение не может быть отправлено. Убедитесь, что в сообщении электронной почты есть действительный получатель**.</span><span class="sxs-lookup"><span data-stu-id="fa08b-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="fa08b-104">Проверьте, существует ли пользователь в группе разрешений " **все пользователи** " (список сведений о пользователях) для этого семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="fa08b-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="fa08b-105">Пример прямого URL-адреса<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/People.aspx? Мембершипграупид = 0</span><span class="sxs-lookup"><span data-stu-id="fa08b-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="fa08b-106">Если пользователь не существует, убедитесь, что пользователь вошел на страницу.</span><span class="sxs-lookup"><span data-stu-id="fa08b-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="fa08b-107">Если это внешний пользователь, убедитесь, что его приглашение принято.</span><span class="sxs-lookup"><span data-stu-id="fa08b-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="fa08b-108">Если пользователь существует в группе разрешений, убедитесь, что адрес электронной почты задан правильно.</span><span class="sxs-lookup"><span data-stu-id="fa08b-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="fa08b-109">Если адрес электронной почты пользователя не задан, создайте пример оповещения для этого пользователя, который принудительно выполняет синхронизацию учетной записи этого пользователя с профилями пользователей SharePoint с этим семейством веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="fa08b-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="fa08b-110">Сообщения от рабочих процессов отправляются администраторам семейства веб-сайтов, но не другим пользователям и отображаются ошибки **http, запрещенные для <span>https:</span>//URL/_vti_bin/Client.XVC.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="fa08b-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="fa08b-111">[В статье отказ в доступе при отправке сообщения электронной почты в группу SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="fa08b-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="fa08b-112">Кроме того, убедитесь, что компонент "семейство веб-сайтов с ограниченным доступом" не активен в **режиме ограниченного доступа** .</span><span class="sxs-lookup"><span data-stu-id="fa08b-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="fa08b-113">Статьи по теме</span><span class="sxs-lookup"><span data-stu-id="fa08b-113">Related topics</span></span>
<span data-ttu-id="fa08b-114">Хотите попробовать Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="fa08b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="fa08b-115">Создание последовательности</span><span class="sxs-lookup"><span data-stu-id="fa08b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="fa08b-116">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="fa08b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


