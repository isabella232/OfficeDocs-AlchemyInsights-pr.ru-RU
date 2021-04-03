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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505701"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="72a6e-102">Восстановление удаленной группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="72a6e-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="72a6e-103">Вы можете восстановить удаленную группу Microsoft 365 или Microsoft Teams в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="72a6e-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="72a6e-104">Чтобы войти в центр администрирования Microsoft 365 и перечислить удаленные группы и группы, перейдите в центр администрирования [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="72a6e-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="72a6e-105">**Примечание:** Войдите в систему с помощью учетной записи, назначенной администратору клиента или роли администратора групп.</span><span class="sxs-lookup"><span data-stu-id="72a6e-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="72a6e-106">Выберите удаленную группу Microsoft 365/Teams, которая будет восстановлена, и щелкните **группу восстановления.**</span><span class="sxs-lookup"><span data-stu-id="72a6e-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="72a6e-107">Если группа не может быть восстановлена из-за конфликтующих smTP-адресов, используйте следующую команду, чтобы найти объект, вызывающий конфликт, и удалить адрес SMTP:</span><span class="sxs-lookup"><span data-stu-id="72a6e-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="72a6e-108">**Примечание:** В некоторых случаях для восстановления группы и всех ее данных может потребоваться до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="72a6e-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="72a6e-109">Дополнительные сведения или сведения о восстановлении групп с помощью PowerShell см. в руб. Восстановление удаленных групп [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="72a6e-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>