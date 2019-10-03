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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376801"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="e0358-102">Управление параметрами и уровнем участия в зале ожидания</span><span class="sxs-lookup"><span data-stu-id="e0358-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="e0358-103">Эти параметры определяют, какие участники собрания ожидают, прежде чем они будут допущены на собрание, и уровень участия, разрешенный им на собрании.</span><span class="sxs-lookup"><span data-stu-id="e0358-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="e0358-104">Вы можете использовать PowerShell, чтобы обновить параметры политики для собраний, которые еще не были реализованы (помечены в ближайшее время) в центре администрирования Teams.</span><span class="sxs-lookup"><span data-stu-id="e0358-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="e0358-105">Ниже приведен пример командлета PowerShell, который позволяет всем пользователям обходить "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="e0358-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="e0358-106">[Автоматически](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) допустить люди — это политика для каждого организатора, которая определяет, присоединяет ли люди непосредственно или ждет, пока пользователь не пройдет проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="e0358-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e0358-107">[Разрешить анонимным пользователям начинать собрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) — это политика организатора, которая определяет, могут ли анонимные пользователи, включая B2B и Федеративные пользователи, присоединиться к собранию пользователя без прошедшего проверку подлинности пользователя из Организации в присутствии.</span><span class="sxs-lookup"><span data-stu-id="e0358-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e0358-108">[Разрешить пользователям с телефонным подключением обходить "зал ожидания"](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) — это политика для каждого организатора, которая определяет, будут ли пользователи, подключающиеся по телефону, напрямую или в зале ожидания, независимо от параметра автоматически допустить **людей** .</span><span class="sxs-lookup"><span data-stu-id="e0358-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e0358-109">[Разрешить организаторов переопределять параметры ожидания](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**ожидается в ближайшее время**) — это политика для каждого организатора, которая определяет, может ли организатор собрания переопределять параметры, заданные администратором автоматически, допустить **людей** и **Разрешить подключение по телефонной линии Пользователи могут обходить зал ожидания** при планировании нового собрания.</span><span class="sxs-lookup"><span data-stu-id="e0358-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e0358-110">**Примечание:** Ознакомьтесь с разделом [Управление политиками собраний в Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , чтобы получить полный обзор политик собраний Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e0358-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="e0358-111">**Пример PowerShell**</span><span class="sxs-lookup"><span data-stu-id="e0358-111">**PowerShell example**</span></span>

<span data-ttu-id="e0358-112">Если вы хотите разрешить всем пользователям, в том числе внешним или анонимным пользователям, обходить его, вы также можете использовать PowerShell для выполнения этой задачи.</span><span class="sxs-lookup"><span data-stu-id="e0358-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="e0358-113">В этом примере показано, как изменить глобальную политику собраний для своей организации.</span><span class="sxs-lookup"><span data-stu-id="e0358-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="e0358-114">Прежде чем приступать к этим изменениям, обязательно ознакомьтесь с документацией, приведенной выше, чтобы убедиться в том, что это позволяет.</span><span class="sxs-lookup"><span data-stu-id="e0358-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="e0358-115">Set — Кстеамсмитингполици — Identity global — Аутоадмиттедусерс "Everyone" — Алловпстнусерстобипасслобби $True</span><span class="sxs-lookup"><span data-stu-id="e0358-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="e0358-116">Дополнительные сведения см. в статье [Set – кстеамсмитингполици](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="e0358-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
