---
title: Восстановление удаленной группы Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645144"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="59d61-102">Восстановление удаленной группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="59d61-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="59d61-103">Вы можете восстановить удаленную группу Microsoft 365 или Microsoft Teams в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="59d61-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="59d61-104">Перейдите в [центр администрирования Microsoft 365,](https://aka.ms/RestoreDeletedGroup) чтобы войти в список удаленных групп и групп.</span><span class="sxs-lookup"><span data-stu-id="59d61-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="59d61-105">**Примечание:** Войдите в систему с помощью учетной записи, назначенной администратору клиента или роли администратора групп.</span><span class="sxs-lookup"><span data-stu-id="59d61-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="59d61-106">Выберите удаленную группу Microsoft 365/Teams, которая будет восстановлена, и щелкните **группу восстановления.**</span><span class="sxs-lookup"><span data-stu-id="59d61-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="59d61-107">Если группа не может быть восстановлена из-за конфликтующих smTP-адресов, используйте следующую команду, чтобы найти объект, вызывающий конфликт, и удалить адрес SMTP:</span><span class="sxs-lookup"><span data-stu-id="59d61-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="59d61-108">**Примечание:** В некоторых случаях для восстановления группы и всех ее данных может потребоваться до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="59d61-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="59d61-109">Дополнительные сведения или сведения о восстановлении групп с помощью PowerShell см. в руб. Восстановление удаленных групп [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="59d61-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>