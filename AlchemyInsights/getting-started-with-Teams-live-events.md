---
title: Начало работы с трансляциями Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677292"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="5b6b5-102">Начало работы с трансляциями Teams</span><span class="sxs-lookup"><span data-stu-id="5b6b5-102">Getting started with Teams live events</span></span>

<span data-ttu-id="5b6b5-103">Трансляции Microsoft Teams — это расширение собраний Teams, с помощью которого можно планировать и проводить мероприятия с трансляцией для крупных аудиторий в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="5b6b5-104">Для создания трансляции необходимо следующее:</span><span class="sxs-lookup"><span data-stu-id="5b6b5-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="5b6b5-105">Сначала убедитесь, что трансляции Teams [доступны в вашей стране или регионе](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability). Трансляции пока недоступны в некоторых странах и регионах.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="5b6b5-106">Если вы назначили лицензии и настроили политики, но по-прежнему не можете создать трансляцию Teams, скорее всего, вы находитесь в стране или регионе, где трансляции пока недоступны.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="5b6b5-107">Лицензия [Office 365 корпоративный E1, E3, E5 либо лицензия Office 365 A3 или A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="5b6b5-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="5b6b5-108">**Примечание**. Из-за недавнего увеличения использования Teams полная настройка при назначении лицензии Teams пользователям может занять около 24 часов.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="5b6b5-109">До этого вы не сможете назначать пользователям политики Teams, а у пользователей может не быть доступа к определенным функциям Teams, таким как звонки или аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="5b6b5-110">Разрешение на [создание трансляций в Центре администрирования Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="5b6b5-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="5b6b5-111">Разрешение на [создание трансляций в Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (для мероприятий, созданных с помощью внешнего вещательного приложения или устройства).</span><span class="sxs-lookup"><span data-stu-id="5b6b5-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="5b6b5-112">Полное участие группы в организации (нельзя использовать гостевые группы или группы из другой организации).</span><span class="sxs-lookup"><span data-stu-id="5b6b5-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="5b6b5-113">В политике собраний Teams необходимо включить планирование частных собраний, демонстрацию экрана и демонстрацию видео по IP.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="5b6b5-114">[Рекомендации](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) по трансляциям Teams.</span><span class="sxs-lookup"><span data-stu-id="5b6b5-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="5b6b5-115">Дополнительные сведения см. в статье [Начало работы с трансляциями Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="5b6b5-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>