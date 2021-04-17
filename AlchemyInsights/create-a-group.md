---
title: Создание группы
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816373"
---
# <a name="create-a-group"></a><span data-ttu-id="06914-102">Создание группы</span><span class="sxs-lookup"><span data-stu-id="06914-102">Create a group</span></span>

<span data-ttu-id="06914-103">В этом разделе описывается создание групп.</span><span class="sxs-lookup"><span data-stu-id="06914-103">This topic describes group creation.</span></span>

<span data-ttu-id="06914-104">**Разрешение на создание группы**</span><span class="sxs-lookup"><span data-stu-id="06914-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="06914-105">Убедитесь, что вы уполномочены создавать новую группу.</span><span class="sxs-lookup"><span data-stu-id="06914-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="06914-106">Глобальные администраторы могут отключить создание групп на портале Azure или панели доступа.</span><span class="sxs-lookup"><span data-stu-id="06914-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="06914-107">Может потребоваться администратор для создания новой группы или для получения соответствующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="06914-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="06914-108">**Управление разрешениями на создание групп**</span><span class="sxs-lookup"><span data-stu-id="06914-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="06914-109">Глобальные администраторы могут управлять разрешениями на создание групп (по соображениям безопасности) или группами Office 365, созданными на портале Azure или панели доступа, выбрав параметры "Пользователи могут создавать группы безопасности на порталах Azure" или "Пользователи могут создавать группы Office 365 в порталах Azure" во всех группах Общего  >  **(Параметры)**.</span><span class="sxs-lookup"><span data-stu-id="06914-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="06914-110">Вы также можете ограничить создание группы, чтобы выбрать группу пользователей, если у вас есть лицензия Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="06914-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="06914-111">**Отключение приветствия для новых членов группы Office 365**</span><span class="sxs-lookup"><span data-stu-id="06914-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="06914-112">Приветствие, отправленное пользователям, добавленным в группы Office 365, может быть отключено путем установки **ЕдинойGroupWelcomeMessageEnabled** для False в Powershell.</span><span class="sxs-lookup"><span data-stu-id="06914-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="06914-113">Подробные сведения об этом параметре см. [здесь](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="06914-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

