---
title: Откат к предыдущей сборке Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 9f6a812def2b46bf32d836781d0336aea5ba3ed1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727832"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="ed576-102">Откат к предыдущей сборке Office</span><span class="sxs-lookup"><span data-stu-id="ed576-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="ed576-103">Инструкции по возврату к более ранним версиям приложений Microsoft 365 см. в статье [Возврат к более ранней версии Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span><span class="sxs-lookup"><span data-stu-id="ed576-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="ed576-104">Чтобы переключиться с одной подписки на Microsoft 365 на другую, см. раздел [Переход на другой план Microsoft 365 для бизнеса](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="ed576-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="ed576-105">Чтобы определить, какой лицензией Office вы пользуетесь, см. статью [Office: Какая у меня версия Office?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span><span class="sxs-lookup"><span data-stu-id="ed576-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="ed576-106">Сведения о том, как определить версию, к которой вы хотите вернуться, см. в статье [Журнал обновлений для приложений Microsoft 365 (по дате)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span><span class="sxs-lookup"><span data-stu-id="ed576-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="ed576-107">Настройте **Целевую_версию**, чтобы вернуться к предыдущей сборке при помощи [Возврат к более ранней версии Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) или [Задержка получения обновлений через Полугодичный канал при использовании Сети доставки содержимого (CDN) Office](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span><span class="sxs-lookup"><span data-stu-id="ed576-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="ed576-108">Когда задана целевая версия, Office обновляется до нее при поиске обновлений.</span><span class="sxs-lookup"><span data-stu-id="ed576-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>