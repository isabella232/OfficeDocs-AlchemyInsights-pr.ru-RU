---
title: Скрытие общедоступных папок
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294649"
---
# <a name="hide-public-folders"></a><span data-ttu-id="bab0c-102">Скрытие общедоступных папок</span><span class="sxs-lookup"><span data-stu-id="bab0c-102">Hide public folders</span></span>

<span data-ttu-id="bab0c-103">**Чтобы скрыть все дерево общедоступных папок**:</span><span class="sxs-lookup"><span data-stu-id="bab0c-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="bab0c-104">Следуйте инструкциям [этой](https://aka.ms/ControlPF) статьи, чтобы скрыть все дерево общедоступных папок для некоторых или всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="bab0c-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="bab0c-105">**Чтобы скрыть определенную общедоступную папку**:</span><span class="sxs-lookup"><span data-stu-id="bab0c-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="bab0c-106">Добавление разрешений для пользователей, которым необходим доступ к общедоступной папке</span><span class="sxs-lookup"><span data-stu-id="bab0c-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="bab0c-107">Удалите для пользователя разрешение **По умолчанию** из списка **разрешений**:</span><span class="sxs-lookup"><span data-stu-id="bab0c-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
