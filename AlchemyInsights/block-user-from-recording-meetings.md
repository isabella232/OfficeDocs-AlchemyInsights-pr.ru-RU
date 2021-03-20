---
title: Блокировка пользователя от записи собраний
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
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897978"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="6d238-102">Блокировка пользователя от записи собраний</span><span class="sxs-lookup"><span data-stu-id="6d238-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="6d238-103">Если необходимо запретить **или заблокировать** запись собраний teams, вы можете сделать это с помощью параметров политики собраний Teams.</span><span class="sxs-lookup"><span data-stu-id="6d238-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="6d238-104">В центре администрирования Microsoft Teams отключите параметр **Разрешить** облачную запись в политике собраний, назначенной этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="6d238-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="6d238-105">Дополнительные новости см. в [руб. Управление политиками собраний в Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="6d238-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="6d238-106">Чтобы проверить, разрешено ли конкретному пользователю записывать собрания teams, используйте диагностику поддержки.</span><span class="sxs-lookup"><span data-stu-id="6d238-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="6d238-107">Запустите новый запрос поддержки и введите в **Diag: Meeting Recording —** диагностика проверит параметры политики для указанного пользователя и определит параметры политики.</span><span class="sxs-lookup"><span data-stu-id="6d238-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="6d238-108">Помните, что для того, чтобы новые параметры политики вступили в силу, может занять несколько часов, поэтому если вы только что в изменились, подождите несколько часов, прежде чем снова запускать диагностику.</span><span class="sxs-lookup"><span data-stu-id="6d238-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="6d238-109">Дополнительные сведения просмотрите [включите или отключите облачную запись.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="6d238-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
