---
title: Устранение неполадок при доступе к сообщениям
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760353"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="b65cc-102">Устранение неполадок в сообщениях отказа в доступе в SharePoint и в центре администрирования OneDrive</span><span class="sxs-lookup"><span data-stu-id="b65cc-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="b65cc-103">Если вы получаете сообщение об отказе в доступе при попытке перейти в центр администрирования SharePoint или OneDrive, убедитесь, что вы [назначили пользователю лицензию](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="b65cc-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="b65cc-104">Если у пользователя есть лицензия, убедитесь, что [ей назначена роль администратора](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , которая может получать доступ к центрам администрирования.</span><span class="sxs-lookup"><span data-stu-id="b65cc-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="b65cc-105">Эта проблема также может возникать, если пользователь удален и повторно создан с тем же именем участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="b65cc-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b65cc-106">Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта).</span><span class="sxs-lookup"><span data-stu-id="b65cc-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b65cc-107">Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID.</span><span class="sxs-lookup"><span data-stu-id="b65cc-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b65cc-108">Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="b65cc-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b65cc-109">Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.</span><span class="sxs-lookup"><span data-stu-id="b65cc-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b65cc-110">Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и [восстановить пользователя в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b65cc-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="b65cc-111">Примечание: Если центр администрирования OneDrive или SharePoint недоступен для нескольких пользователей, у которых ранее был доступ, может возникнуть временная ошибка службы.</span><span class="sxs-lookup"><span data-stu-id="b65cc-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="b65cc-112">[Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b65cc-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


