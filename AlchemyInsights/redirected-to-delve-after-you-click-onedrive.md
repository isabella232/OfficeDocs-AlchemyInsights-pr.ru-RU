---
title: Веб-приложение OneDrive для бизнеса, перенаправляемое в delve
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776393"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="478d7-102">Перенаправление на delve после нажатия кнопки OneDrive</span><span class="sxs-lookup"><span data-stu-id="478d7-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="478d7-103">Ознакомьтесь с подробным [руководством по устранению неполадок](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="478d7-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="478d7-104">Чтобы устранить эту проблему, администратор должен предоставить пользователям право на создание сайта личных сайтов.</span><span class="sxs-lookup"><span data-stu-id="478d7-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="478d7-105">Это связано с тем, что страница OneDrive для бизнеса создана на личных сайтах.</span><span class="sxs-lookup"><span data-stu-id="478d7-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="478d7-106">Чтобы предоставить это право, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="478d7-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="478d7-107">В центре администрирования SharePoint выберите **Профили пользователей**.</span><span class="sxs-lookup"><span data-stu-id="478d7-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="478d7-108">В разделе **люди** выберите **Управление разрешениями пользователей**.</span><span class="sxs-lookup"><span data-stu-id="478d7-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="478d7-109">Добавьте пользователей, которым требуются разрешения на создание сайта личных сайтов.</span><span class="sxs-lookup"><span data-stu-id="478d7-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="478d7-110">По умолчанию этому параметру присвоено значение **все, кроме внешних пользователей**.</span><span class="sxs-lookup"><span data-stu-id="478d7-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="478d7-111">После добавления пользователя, пользователей или группы убедитесь, что выбраны добавленные пользователи, пользователи или группы, перейдите к разделу **разрешения** , а затем установите флажок **создать личный сайт (требуется для личного хранилища, канала новостей и контента)**.</span><span class="sxs-lookup"><span data-stu-id="478d7-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="478d7-112">Нажмите кнопку **ОК**, а затем попросите пользователя открыть страницу OneDrive, чтобы создать сайт.</span><span class="sxs-lookup"><span data-stu-id="478d7-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
