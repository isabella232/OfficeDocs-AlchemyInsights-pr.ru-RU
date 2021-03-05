---
title: Блокировка пользовательских подписей электронной почты
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464874"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="eddd1-102">Блокировка пользовательских подписей электронной почты</span><span class="sxs-lookup"><span data-stu-id="eddd1-102">Block user-made email signatures</span></span>

<span data-ttu-id="eddd1-103">Следующее решение применяется только к подписям электронной почты, созданным в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="eddd1-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="eddd1-104">Подписи в приложении Outlook можно заблокировать только в том случае, если у вас есть локальное Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="eddd1-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="eddd1-105">В центре администрирования выберите **центры администрирования**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="eddd1-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="eddd1-106">Щелкните **разрешения**  >  **Outlook Web App политик**.</span><span class="sxs-lookup"><span data-stu-id="eddd1-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="eddd1-107">Выберите политику, а затем нажмите значок карандаша, чтобы изменить ее.</span><span class="sxs-lookup"><span data-stu-id="eddd1-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="eddd1-108">Щелкните   >  **функции Дополнительные параметры**.</span><span class="sxs-lookup"><span data-stu-id="eddd1-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="eddd1-109">В **пользовательском окне** очистить **поле** подписи электронной почты, а затем нажмите **кнопку Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="eddd1-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="eddd1-110">**Важно:** Если перед очисткой этого чека была добавлена подпись, пользователь все равно сможет ее использовать.</span><span class="sxs-lookup"><span data-stu-id="eddd1-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="eddd1-111">Попросите их удалить его.</span><span class="sxs-lookup"><span data-stu-id="eddd1-111">Ask them to remove it.</span></span>
