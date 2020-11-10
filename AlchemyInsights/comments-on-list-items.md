---
title: Комментарии к элементам списка
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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947505"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="ce973-102">Комментарии к элементам списка</span><span class="sxs-lookup"><span data-stu-id="ce973-102">Comments on List items</span></span>

<span data-ttu-id="ce973-103">В скором времени пользователи смогут добавлять и удалять комментарии к элементам списка.</span><span class="sxs-lookup"><span data-stu-id="ce973-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="ce973-104">Пользователи могут просматривать все комментарии к элементу списка и фильтровать представления, которые отображают комментарии или действия, связанные с элементом.</span><span class="sxs-lookup"><span data-stu-id="ce973-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="ce973-105">**Время** :</span><span class="sxs-lookup"><span data-stu-id="ce973-105">**Timing** :</span></span>

<span data-ttu-id="ce973-106">**Целевой выпуск** : постепенное развертывание в середине от октября и ожидаемое выполнение за середину ноября</span><span class="sxs-lookup"><span data-stu-id="ce973-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="ce973-107">**Стандартный выпуск** : постепенное развертывание в середине за ноябрь и ожидаемое завершение на ранних декабря</span><span class="sxs-lookup"><span data-stu-id="ce973-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="ce973-108">**Развертывание** : нацеленный выпуск для всей Организации</span><span class="sxs-lookup"><span data-stu-id="ce973-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="ce973-109">Перед добавлением и удалением комментариев пользователям необходимо отметить следующее:</span><span class="sxs-lookup"><span data-stu-id="ce973-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="ce973-110">Комментарии следуют параметрам разрешений, встроенным в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ce973-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="ce973-111">Для классических списков, которые еще не созданы для отображения в современных пользовательских интерфейсах, таких как списки задач, эта функция комментирования не будет создана.</span><span class="sxs-lookup"><span data-stu-id="ce973-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="ce973-112">Комментирование списков в Microsoft Teams недоступно в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="ce973-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="ce973-113">Комментарии не индексируются службой поиска.</span><span class="sxs-lookup"><span data-stu-id="ce973-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="ce973-114">Администраторы могут отключить эту функцию на уровне Организации, изменив параметр **комментсонлиститемсдисаблед** в командлете **Set – SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ce973-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="ce973-115">В настоящее время невозможно отключить комментирование на уровне сайта или списка.</span><span class="sxs-lookup"><span data-stu-id="ce973-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="ce973-116">Мы надеемся, что эти элементы управления будут впоследствии обновлены в течение первого квартала 2021.</span><span class="sxs-lookup"><span data-stu-id="ce973-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
