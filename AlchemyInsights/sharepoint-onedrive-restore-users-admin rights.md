---
title: Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354810"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="29da0-102">Устранение неполадок, связанных с доступом запрещенных сообщений для сайтов OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="29da0-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="29da0-103">Эта проблема чаще всего возникает, когда пользователь удаляется и повторно создается с тем же именем участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="29da0-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="29da0-104">Новая учетная запись создается с использованием другого значения идентификатора PUID (уникального идентификатора паспорта).</span><span class="sxs-lookup"><span data-stu-id="29da0-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="29da0-105">Когда пользователь пытается получить доступ к семейству веб-сайтов или их OneDrive, у пользователя будет неправильный идентификатор PUID.</span><span class="sxs-lookup"><span data-stu-id="29da0-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="29da0-106">Второй сценарий включает синхронизацию службы каталогов с подразделением Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="29da0-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="29da0-107">Если пользователи уже выполнили вход в SharePoint, а затем перемещаются в другое подразделение и повторно синхронизируются с SharePoint, они могут столкнуться с этой проблемой.</span><span class="sxs-lookup"><span data-stu-id="29da0-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="29da0-108">Чтобы устранить эту проблему, необходимо восстановить исходное имя участника-пользователя, выполнив действия, описанные в этой статье, и[восстановить пользователя в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="29da0-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="29da0-109">После этого вы можете проверить, есть ли у пользователя права администратора на сайте OneDrive, выполнив действия, описанные в статье [Добавление администратора для onedrive пользователя](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="29da0-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="29da0-110">Более подробную информацию об уровнях разрешений можно узнать в статье, посвященной [уровням разрешений в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="29da0-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
