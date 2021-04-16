---
title: OneDrive для бизнеса Web OneDrive перенаправляет в Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800002"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="14ba4-102">Перенаправлено в Delve после нажатия OneDrive</span><span class="sxs-lookup"><span data-stu-id="14ba4-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="14ba4-103">См. в нашем [подробном руководстве по устранению неполадок.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="14ba4-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="14ba4-104">Чтобы устранить эту проблему, администратор должен предоставить пользователям право создавать свой сайт "Мои сайты".</span><span class="sxs-lookup"><span data-stu-id="14ba4-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="14ba4-105">Это происходит потому, что страница OneDrive для бизнеса создается на моих сайтах.</span><span class="sxs-lookup"><span data-stu-id="14ba4-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="14ba4-106">Чтобы предоставить это право, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="14ba4-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="14ba4-107">В центре администрирования SharePoint щелкните **профили пользователей.**</span><span class="sxs-lookup"><span data-stu-id="14ba4-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="14ba4-108">В разделе **Люди** нажмите **кнопку Управление разрешениями пользователей**.</span><span class="sxs-lookup"><span data-stu-id="14ba4-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="14ba4-109">Добавьте пользователей, которым требуются разрешения на создание сайта My Sites.</span><span class="sxs-lookup"><span data-stu-id="14ba4-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="14ba4-110">По умолчанию этот параметр заданной для **всех, кроме внешних пользователей.**</span><span class="sxs-lookup"><span data-stu-id="14ba4-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="14ba4-111">После добавления пользователя, пользователей или группы убедитесь, что добавленный пользователь, пользователи или  группа выбраны, прокрутите в раздел разрешений, а затем выберите контрольный ящик рядом с Create Personal Site (необходимый для личного хранения, ленты новостей и **контента)**.</span><span class="sxs-lookup"><span data-stu-id="14ba4-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="14ba4-112">Нажмите **кнопку ОК,** а затем перейдите на страницу OneDrive, чтобы создать сайт.</span><span class="sxs-lookup"><span data-stu-id="14ba4-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
