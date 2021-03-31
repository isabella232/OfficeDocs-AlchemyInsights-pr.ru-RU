---
title: 126 Получение почтового ящика невозможно найти ошибку в OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426675"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="14aa7-102">Получение почтового ящика, не найденного в Outlook в Интернете?</span><span class="sxs-lookup"><span data-stu-id="14aa7-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="14aa7-103">Если вы используете Outlook в Интернете и  не можете найти почтовый ящик из-за ошибки, учетная запись, которую вы использовали для подключения к Outlook в Интернете, не имеет лицензии Exchange Online, поэтому почтовый ящик не связан с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="14aa7-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="14aa7-104">Администратор может назначить лицензию вашей учетной записи, следуя следующим шагам:</span><span class="sxs-lookup"><span data-stu-id="14aa7-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="14aa7-105">Откройте центр  [администрирования Microsoft 365](https://portal.office.com/adminportal/home#/homepage) и перейдите к активным пользователям в разделе **Пользователи** и выберите пользователя, который видит ошибку.</span><span class="sxs-lookup"><span data-stu-id="14aa7-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="14aa7-106">На открываемой странице пользователя  перейдите в раздел Лицензии и приложения, выберите соответствующее значение Location и назначьте лицензию, содержаную Exchange Online (разместите лицензию, чтобы увидеть ее сведения). </span><span class="sxs-lookup"><span data-stu-id="14aa7-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="14aa7-107">После завершения нажмите кнопку **Сохранить изменения**.</span><span class="sxs-lookup"><span data-stu-id="14aa7-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="14aa7-108">В некоторых случаях, если лицензия уже назначена учетной записи пользователя, удаление и перенана присвоение лицензии помогает устранить проблему и правильно подготовить ее в системе:</span><span class="sxs-lookup"><span data-stu-id="14aa7-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="14aa7-109">Проверьте, являются ли подписки M365 Exchange Online (и другие, если у вас есть) текущими и не истекли.</span><span class="sxs-lookup"><span data-stu-id="14aa7-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="14aa7-110">После того как вы убедились, что срок действия подписки не истек, а для учетной записи пользователя назначена действительная лицензия, может потребоваться до 24 часов, поэтому может потребоваться дождаться решения проблемы.</span><span class="sxs-lookup"><span data-stu-id="14aa7-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="14aa7-111">Дополнительные сведения см. в [дополнительных сведениях о назначении лицензий и управлении ими.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="14aa7-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>