---
title: Устранение неполадок в доступе, отказано в сообщениях
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707967"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="c2550-102">Устранение неполадок с отказом в доступе к сообщениям в Центре администрирования Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="c2550-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="c2550-103">Если при попытке просмотра в Центре администрирования Sharepoint/OneDrive вы получаете сообщение об отказе в доступе, убедитесь, что вы назначите пользователю [лицензию.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="c2550-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="c2550-104">Если у пользователя есть лицензия, необходимо [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) также убедиться, что им назначена роль администратора, которая может получить доступ к центрам администрирования.</span><span class="sxs-lookup"><span data-stu-id="c2550-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="c2550-105">Эта проблема также может возникать, когда пользователь удаляется и повторно создается с тем же основным именем пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="c2550-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c2550-106">Новая учетная запись создается с помощью другого значения PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="c2550-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c2550-107">Когда пользователь пытается получить доступ к коллекции сайтов или к oneDrive, у пользователя имеется неправильный PUID.</span><span class="sxs-lookup"><span data-stu-id="c2550-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c2550-108">Второй сценарий включает синхронизацию каталогов с организационным подразделением Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="c2550-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c2550-109">Если пользователи уже подписались на SharePoint, а затем перемещаются в другой OU и повторно с SharePoint, у них может возникнуть эта проблема.</span><span class="sxs-lookup"><span data-stu-id="c2550-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c2550-110">Чтобы устранить эту проблему, необходимо восстановить исходный upN с помощью действий в статье [Восстановление пользователя в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="c2550-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="c2550-111">Примечание. Если центр администрирования OneDrive или SharePoint не доступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная проблема с обслуживанием.</span><span class="sxs-lookup"><span data-stu-id="c2550-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="c2550-112">[Проверьте панель мониторинга состояния службы.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="c2550-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


