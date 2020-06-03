---
title: Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511197"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="bef9e-102">Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="bef9e-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="bef9e-103">Эта проблема чаще всего возникает, когда пользователь удаляется и повторно создается с тем же именем участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="bef9e-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="bef9e-104">Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта).</span><span class="sxs-lookup"><span data-stu-id="bef9e-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="bef9e-105">Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID.</span><span class="sxs-lookup"><span data-stu-id="bef9e-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="bef9e-106">Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="bef9e-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="bef9e-107">Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.</span><span class="sxs-lookup"><span data-stu-id="bef9e-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="bef9e-108">Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и [восстановить пользователя в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="bef9e-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="bef9e-109">Если не удается восстановить исходного пользователя, необходимо удалить старого пользователя с сайта OneDrive, выполнив указанные ниже действия, [удалить пользователя из списка сведений о пользователе]().</span><span class="sxs-lookup"><span data-stu-id="bef9e-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="bef9e-110">После этого вы можете проверить, есть ли у пользователя права администратора на сайте OneDrive, выполнив действия, описанные в статье [Добавление администратора для onedrive пользователя](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="bef9e-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="bef9e-111">Более подробную информацию об уровнях разрешений можно узнать в статье, посвященной [уровням разрешений в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="bef9e-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
