---
title: Веб-приложение OneDrive для бизнеса, перенаправляемое в delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722823"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="e5205-102">Перенаправление на delve после нажатия кнопки OneDrive</span><span class="sxs-lookup"><span data-stu-id="e5205-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="e5205-103">Ознакомьтесь с подробным [руководством по устранению неполадок](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="e5205-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="e5205-104">Чтобы устранить эту проблему, администратор должен предоставить пользователям право на создание сайта личных сайтов.</span><span class="sxs-lookup"><span data-stu-id="e5205-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="e5205-105">Это связано с тем, что страница OneDrive для бизнеса создана на личных сайтах.</span><span class="sxs-lookup"><span data-stu-id="e5205-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="e5205-106">Чтобы предоставить это право, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="e5205-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="e5205-107">В центре администрирования SharePoint выберите **Профили пользователей**.</span><span class="sxs-lookup"><span data-stu-id="e5205-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="e5205-108">В разделе **люди** выберите **Управление разрешениями пользователей**.</span><span class="sxs-lookup"><span data-stu-id="e5205-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="e5205-109">Добавьте пользователей, которым требуются разрешения на создание сайта личных сайтов.</span><span class="sxs-lookup"><span data-stu-id="e5205-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="e5205-110">По умолчанию этому параметру присвоено значение **все, кроме внешних пользователей**.</span><span class="sxs-lookup"><span data-stu-id="e5205-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="e5205-111">После добавления пользователя, пользователей или группы убедитесь, что выбраны добавленные пользователи, пользователи или группы, перейдите к разделу **разрешения** , а затем установите флажок **создать личный сайт (требуется для личного хранилища, канала новостей и контента)**.</span><span class="sxs-lookup"><span data-stu-id="e5205-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="e5205-112">Нажмите кнопку **ОК**, а затем попросите пользователя открыть страницу OneDrive, чтобы создать сайт.</span><span class="sxs-lookup"><span data-stu-id="e5205-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
