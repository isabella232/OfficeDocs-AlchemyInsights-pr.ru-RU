---
title: Комментарии к элементов списка
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724167"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="332bc-102">Комментарии к элементов списка</span><span class="sxs-lookup"><span data-stu-id="332bc-102">Comments on List items</span></span>

<span data-ttu-id="332bc-103">Пользователи могут просматривать все комментарии к элементу списка и фильтровать их между представлениями, которые показывают комментарии или действия, связанные с элементом.</span><span class="sxs-lookup"><span data-stu-id="332bc-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="332bc-104">Чтобы пользователи могли добавлять и удалять комментарии, необходимо отметить следующее:</span><span class="sxs-lookup"><span data-stu-id="332bc-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="332bc-105">Комментарии следуют за настройками разрешений, характерных для SharePoint.</span><span class="sxs-lookup"><span data-stu-id="332bc-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="332bc-106">Классические списки, которые еще не были встроены в современные пользовательские интерфейсы, такие как списки задач, не будут иметь этой функции коммента.</span><span class="sxs-lookup"><span data-stu-id="332bc-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="332bc-107">Комментарии к спискам в Teams недоступны в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="332bc-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="332bc-108">Комментарии не индексироваться поиском.</span><span class="sxs-lookup"><span data-stu-id="332bc-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="332bc-109">Администраторы могут отключить эту функцию на уровне организации, изменив параметр **CommentsOnListItemsDisabled** в **параметре Set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="332bc-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="332bc-110">В настоящее время невозможно отключить комментарии на уровне сайта или списка.</span><span class="sxs-lookup"><span data-stu-id="332bc-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="332bc-111">Мы надеемся, что эти элементы управления будут обновлены позже, скорее всего, в первом квартале 2021 г.</span><span class="sxs-lookup"><span data-stu-id="332bc-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
