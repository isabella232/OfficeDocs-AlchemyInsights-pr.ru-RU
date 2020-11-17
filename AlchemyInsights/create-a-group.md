---
title: Создание группы
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086393"
---
# <a name="create-a-group"></a><span data-ttu-id="ea0ab-102">Создание группы</span><span class="sxs-lookup"><span data-stu-id="ea0ab-102">Create a group</span></span>

<span data-ttu-id="ea0ab-103">В этом разделе описывается создание групп.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-103">This topic describes group creation.</span></span>

<span data-ttu-id="ea0ab-104">**Разрешение на создание группы**</span><span class="sxs-lookup"><span data-stu-id="ea0ab-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="ea0ab-105">Убедитесь, что у вас есть разрешение на создание новой группы.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="ea0ab-106">Глобальные администраторы могут отключить создание групп на портале или панели доступа Azure.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="ea0ab-107">Возможно, вам потребуется администратор, чтобы создать новую группу или предоставить вам соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="ea0ab-108">**Управление разрешениями на создание групп**</span><span class="sxs-lookup"><span data-stu-id="ea0ab-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="ea0ab-109">Глобальные администраторы могут управлять разрешениями на создание групп (по причинам, связанным с безопасностью) или группами Office 365, созданными на портале или панели доступа Azure, выбрав "пользователи могут создавать группы безопасности в порталах Azure" или "пользователи могут создавать группы Office 365 в порталах Azure" во **всех группах**  >  **Общие (параметры)**.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="ea0ab-110">Вы также можете ограничить создание групп, чтобы выбрать группу пользователей, если у вас есть лицензия Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="ea0ab-111">**Отключение уведомления приветствия для новых участников группы Office 365**</span><span class="sxs-lookup"><span data-stu-id="ea0ab-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="ea0ab-112">Уведомление о приглашении, отправленное пользователям, добавленным в группы Office 365, можно отключить, задав для **UnifiedGroupWelcomeMessageEnabled** значение false в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="ea0ab-113">В этой [статье](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)рассказывается о данном параметре.</span><span class="sxs-lookup"><span data-stu-id="ea0ab-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

