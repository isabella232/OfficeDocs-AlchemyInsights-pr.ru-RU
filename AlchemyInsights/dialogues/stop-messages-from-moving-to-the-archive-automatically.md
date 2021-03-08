---
title: Автоматическое перемещение сообщений в архив
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522419"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="ef0e1-102">Автоматическое перемещение сообщений в архив</span><span class="sxs-lookup"><span data-stu-id="ef0e1-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="ef0e1-103">Если вы используете политику хранения, вы можете изменить возраст хранения в этой политике, чтобы автоматически не мешать архивам сообщений.</span><span class="sxs-lookup"><span data-stu-id="ef0e1-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="ef0e1-104">Вот как это сделать:</span><span class="sxs-lookup"><span data-stu-id="ef0e1-104">Here's how:</span></span>

1. <span data-ttu-id="ef0e1-105">В центре [администрирования Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)выберите **теги** хранения соответствия  >  требованиям.</span><span class="sxs-lookup"><span data-stu-id="ef0e1-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="ef0e1-106">Найдите тег "Перемещение в архив".</span><span class="sxs-lookup"><span data-stu-id="ef0e1-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="ef0e1-107">В теге хранения измените период хранения  (период архива), чтобы не останавливать автоматические архивы элементов политикой хранения.</span><span class="sxs-lookup"><span data-stu-id="ef0e1-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="ef0e1-108">Это изменит параметр архива для всех почтовых ящиков с помощью этого тега хранения, примененного к ним.</span><span class="sxs-lookup"><span data-stu-id="ef0e1-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
