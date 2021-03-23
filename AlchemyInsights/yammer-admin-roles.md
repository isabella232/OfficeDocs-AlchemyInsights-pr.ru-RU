---
title: Об администраторах Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995292"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="8d4f0-102">Об администраторах Yammer</span><span class="sxs-lookup"><span data-stu-id="8d4f0-102">About Yammer admins</span></span>

<span data-ttu-id="8d4f0-103">**Сетевые администраторы**</span><span class="sxs-lookup"><span data-stu-id="8d4f0-103">**Network admins**</span></span>

<span data-ttu-id="8d4f0-104">Глобальные администраторы автоматически продвигаются к роли "Проверенный администратор" в сети Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="8d4f0-105">В следующих случаях эта акция может происходить неправильно:</span><span class="sxs-lookup"><span data-stu-id="8d4f0-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="8d4f0-106">Существует несколько сетей Yammer, и администратор подписывался не в ту.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="8d4f0-107">[Консолидация](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) сети необходима для получения одной сети Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="8d4f0-108">Используется Azure PIM.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-108">Azure PIM is being used.</span></span> <span data-ttu-id="8d4f0-109">Пользователь может не быть повышен до глобального администратора достаточно долго для продвижения по службе.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="8d4f0-110">Возможно, эта проблема будет решаться в будущем обновлении Yammer, но лучше продвигать пользователей к глобальному администратору вручную.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="8d4f0-111">Существует проблема синхронизации с сетью Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="8d4f0-112">В этом случае для дальнейшего расследования потребуется запрос на поддержку.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="8d4f0-113">Дополнительные сведения о ролях администратора Yammer см. в рублях [Управление администраторами Yammer.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="8d4f0-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="8d4f0-114">**Администраторы групп**</span><span class="sxs-lookup"><span data-stu-id="8d4f0-114">**Group admins**</span></span>

<span data-ttu-id="8d4f0-115">Администраторы групп для подключенных групп Microsoft 365 синхронизируются с членством в группах из Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="8d4f0-116">Для больших групп эта синхронизация может занять длительный период.</span><span class="sxs-lookup"><span data-stu-id="8d4f0-116">For large groups, this sync can take an extended period.</span></span>
