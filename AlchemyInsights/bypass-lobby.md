---
title: Обход "зал ожидания"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889095"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="6ebf5-102">Управление параметрами и уровнем участия в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6ebf5-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="6ebf5-103">Если вы хотите разрешить всем пользователям, в том числе пользователям с телефонным подключением, внешним пользователям и анонимным пользователям, **обходить**эту задачу с помощью PowerShell, используйте PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="6ebf5-104">В этом примере показано, как изменить глобальную политику собраний для своей организации.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="6ebf5-105">Для этого командлета в настоящее время требуется использование модуля PowerShell Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="6ebf5-106">Чтобы приступить к настройке для использования этого командлета, изучите [Управление политиками с помощью PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="6ebf5-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="6ebf5-107">После настройки политики ее необходимо применить к пользователям; Если вы изменили глобальную политику, она будет автоматически применена к пользователям.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="6ebf5-108">Для вступления в силу любых изменений политики необходимо подождать не менее **4 часов до 24 часов** , чтобы политики вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="6ebf5-109">Прежде чем вносить эти изменения, ознакомьтесь с приведенной ниже документацией, чтобы убедиться в том, что это позволяет.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="6ebf5-110">Общие сведения об элементах управления политикой для собраний в Teams</span><span class="sxs-lookup"><span data-stu-id="6ebf5-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="6ebf5-111">Эти параметры определяют, какие участники собрания ожидают, прежде чем они будут допущены на собрание, и уровень участия, разрешенный им на собрании.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="6ebf5-112">Вы можете использовать PowerShell, чтобы обновить параметры политики для собраний, которые еще не были реализованы (помечены в ближайшее время) в центре администрирования Teams.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="6ebf5-113">Ниже приведен пример командлета PowerShell, который позволяет всем пользователям обходить "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="6ebf5-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="6ebf5-114">[Автоматически](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) допустить люди — это политика для каждого организатора, которая определяет, присоединяет ли люди непосредственно или ждет, пока пользователь не пройдет проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="6ebf5-115">[Разрешить анонимным пользователям начинать собрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) — это политика организатора, которая определяет, могут ли анонимные пользователи, включая B2B и Федеративные пользователи, присоединиться к собранию пользователя без прошедшего проверку подлинности пользователя из Организации в присутствии.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="6ebf5-116">[Разрешить пользователям с телефонным подключением обходить "зал ожидания"](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) — это политика для каждого организатора, которая определяет, будут ли пользователи, подключающиеся по телефону, напрямую или в зале ожидания, независимо от параметра автоматически допустить **людей** .</span><span class="sxs-lookup"><span data-stu-id="6ebf5-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="6ebf5-117">[Разрешить организаторов переопределять параметры ожидания](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**ожидается**) — это политика для каждого организатора, которая определяет, может ли организатор собрания переопределять параметры, заданные администратором **автоматически** , допустить людей и **разрешать пользователям с телефонным подключением обходить** свое время ожидания при планировании нового собрания.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="6ebf5-118">**Примечание:** Ознакомьтесь с разделом [Управление политиками собраний в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , чтобы получить полный обзор политик собраний Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6ebf5-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
