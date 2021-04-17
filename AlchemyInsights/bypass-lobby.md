---
title: Вестибюль обхода
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820047"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="f8154-102">Контроль параметров лобби и уровня участия в Teams</span><span class="sxs-lookup"><span data-stu-id="f8154-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="f8154-103">Если вы хотите разрешить всем пользователям, включая пользователей dial-in, внешних и анонимных, обходить **лобби,** используйте PowerShell для выполнения этой задачи.</span><span class="sxs-lookup"><span data-stu-id="f8154-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="f8154-104">Вот пример изменения глобальной политики собраний для организации.</span><span class="sxs-lookup"><span data-stu-id="f8154-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="f8154-105">Этот командлет в настоящее время требует использования модуля Skype для бизнеса PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f8154-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="f8154-106">Чтобы настроиться на использование этого комлета, ознакомьтесь с политиками [управления с помощью PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="f8154-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="f8154-107">После того как вы настроили политику, ее необходимо применить к пользователям; или, если вы изменили глобальную политику, она будет автоматически применяться к пользователям.</span><span class="sxs-lookup"><span data-stu-id="f8154-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="f8154-108">Для любых изменений политики необходимо подождать не менее 4 часов до **24** часов, чтобы политики вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="f8154-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="f8154-109">Не забудьте просмотреть ниже документацию, прежде чем вносить эти изменения, чтобы точно понять, что это позволяет.</span><span class="sxs-lookup"><span data-stu-id="f8154-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="f8154-110">Понимание элементов управления политикой лоббирования в собраниях teams</span><span class="sxs-lookup"><span data-stu-id="f8154-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="f8154-111">Эти параметры контролируют, какие участники собраний ждут в вестибюле, прежде чем они будут допущены к собранию, и уровень участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="f8154-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="f8154-112">Вы можете использовать PowerShell для обновления параметров политики собраний, которые еще не реализованы (помечены как "скоро") в центре администрирования Teams.</span><span class="sxs-lookup"><span data-stu-id="f8154-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="f8154-113">См. ниже, например, cmdlet PowerShell, который позволяет всем пользователям обходить вестибюль.</span><span class="sxs-lookup"><span data-stu-id="f8154-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="f8154-114">[Автоматически допускается, что](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) люди являются политикой, которая контролирует, присоединяются ли люди к собранию напрямую или ждут в вестибюле, пока они не будут допущены пользователем с проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="f8154-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="f8154-115">[Разрешить](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) анонимным людям начинать собрание — это политика для каждого организатора, которая контролирует, могут ли анонимные люди, включая B2B и федерабельных пользователей, присоединяться к собранию пользователя без проверки подлинности пользователя из организации, которая присутствовала на собрании.</span><span class="sxs-lookup"><span data-stu-id="f8154-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="f8154-116">[Разрешить](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) пользователям набора номеров обход вестибюля **(в** ближайшее время) — это политика для каждого организатора, которая  контролирует, присоединяются ли люди, которые звонят по телефону, непосредственно к собранию или ждут в вестибюле независимо от параметра автоматически допуска людей.</span><span class="sxs-lookup"><span data-stu-id="f8154-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="f8154-117">Разрешить организаторам переопределять параметры лобби (в ближайшее **время)**— это политика для каждого организатора,  которая контролирует,  может ли организатор собрания переопределять параметры лобби, установленные администратором в Автоматическом впуске людей, и разрешить пользователям в диалоговом режиме обход вестибюля при запланировании нового собрания. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)</span><span class="sxs-lookup"><span data-stu-id="f8154-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="f8154-118">**Примечание:** Ознакомьтесь [с политиками управления собраниями в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) для полного обзора политик собраний Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f8154-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
