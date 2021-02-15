---
title: Синхронизация группы
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243923"
---
# <a name="group-sync"></a><span data-ttu-id="e23ff-102">Синхронизация группы</span><span class="sxs-lookup"><span data-stu-id="e23ff-102">Group sync</span></span>

<span data-ttu-id="e23ff-103">В этой статье приведены инструкции по синхронизации групп.</span><span class="sxs-lookup"><span data-stu-id="e23ff-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="e23ff-104">Если глобальный администратор или владелец группы не может изменить свойства группы или добавить участников на портале Azure, убедитесь, что главным источником для группы является Azure Active Directory (Azure AD), чтобы глобальный администратор или владелец группы могли изменить группу.</span><span class="sxs-lookup"><span data-stu-id="e23ff-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="e23ff-105">Перед удалением синхронизированной группы в Azure AD [удалите все назначенные лицензии](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced), чтобы избежать ошибок.</span><span class="sxs-lookup"><span data-stu-id="e23ff-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="e23ff-106">Сведения о том, как синхронизировать пользователей, группы и контакты, см. в статье [Синхронизация Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), а также в статье [Синхронизация локальной группы с Azure с помощью Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support), чтобы синхронизировать локальные группы с помощью AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e23ff-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="e23ff-107">Чтобы устранить распространенные ошибки во время синхронизации, следуйте инструкциям статьи [Устранение ошибок синхронизации](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="e23ff-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

