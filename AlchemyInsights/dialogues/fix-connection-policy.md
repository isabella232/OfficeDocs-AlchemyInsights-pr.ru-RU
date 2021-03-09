---
title: Исправлена политика подключения
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
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568686"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="c1ef6-102">Исправлена политика подключения</span><span class="sxs-lookup"><span data-stu-id="c1ef6-102">Fix connection policy</span></span>

<span data-ttu-id="c1ef6-103">Электронная почта была помечена безопасной и доставлена в почтовый ящик пользователя, так как ip-адрес отправки был помечен безопасно в политике фильтра подключения.</span><span class="sxs-lookup"><span data-stu-id="c1ef6-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="c1ef6-104">Чтобы просмотреть политику, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="c1ef6-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="c1ef6-105">Перейдите в Центр обеспечения безопасности [Office 365 &,](https://go.microsoft.com/fwlink/p/?linkid=2077143)а затем перейдите в центр по борьбе со спамом политики управления   >    >  [угрозами.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="c1ef6-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="c1ef6-106">На **вкладке Custom** выберите политику **фильтра подключения** и выберите политику **редактирования.**</span><span class="sxs-lookup"><span data-stu-id="c1ef6-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="c1ef6-107">Просмотрите **список IP-адресов.**</span><span class="sxs-lookup"><span data-stu-id="c1ef6-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="c1ef6-108">Узнайте, **включен ли безопасный** список.</span><span class="sxs-lookup"><span data-stu-id="c1ef6-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c1ef6-109">Корпорация Майкрософт использует сторонние источники надежных отправителей.</span><span class="sxs-lookup"><span data-stu-id="c1ef6-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="c1ef6-110">Если **включен безопасный** список, эти доверенные отправители не по ошибке помечены как спам.</span><span class="sxs-lookup"><span data-stu-id="c1ef6-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="c1ef6-111">Я рекомендую выбрать этот параметр, так как это уменьшит количество ложных срабатывающих сообщений (хорошая почта, классифицируется как спам), которые вы получаете.</span><span class="sxs-lookup"><span data-stu-id="c1ef6-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
