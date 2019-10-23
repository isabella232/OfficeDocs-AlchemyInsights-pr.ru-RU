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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637790"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="0487a-102">Управление параметрами и уровнем участия в зале ожидания</span><span class="sxs-lookup"><span data-stu-id="0487a-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="0487a-103">Если вы хотите разрешить всем пользователям, в том числе пользователям с телефонным подключением, внешним пользователям и анонимным пользователям обходить свое время ожидания, вы можете использовать PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0487a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="0487a-104">Ниже приведен пример изменения глобальной политики собраний для Организации.</span><span class="sxs-lookup"><span data-stu-id="0487a-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="0487a-105">Для этого командлета в настоящее время требуется использование модуля PowerShell Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0487a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="0487a-106">Чтобы запустить программу установки для использования этого командлета, изучите Управление политиками с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0487a-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="0487a-107">Можно настроить новую политику, которая затем потребуется применить к пользователям.</span><span class="sxs-lookup"><span data-stu-id="0487a-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="0487a-108">Если вы измените глобальную политику, она будет автоматически применена к пользователям.</span><span class="sxs-lookup"><span data-stu-id="0487a-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="0487a-109">При изменении политики необходимо подождать не менее 4 часов и до 24 часов, чтобы политики вступили в силу.</span><span class="sxs-lookup"><span data-stu-id="0487a-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="0487a-110">Прежде чем вносить эти изменения, ознакомьтесь с приведенной ниже документацией, чтобы убедиться в том, что это позволяет.</span><span class="sxs-lookup"><span data-stu-id="0487a-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="0487a-111">Общие сведения об элементах управления политикой для собраний в Teams</span><span class="sxs-lookup"><span data-stu-id="0487a-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="0487a-112">[Автоматически](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) допустить люди — это политика для каждого организатора, которая определяет, присоединяет ли люди непосредственно или ждет, пока пользователь не пройдет проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="0487a-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="0487a-113">[Разрешить анонимным пользователям начинать собрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) — это политика организатора, которая определяет, могут ли анонимные пользователи, включая B2B и Федеративные пользователи, присоединиться к собранию пользователя без прошедшего проверку подлинности пользователя из Организации в присутствии.</span><span class="sxs-lookup"><span data-stu-id="0487a-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="0487a-114">[Разрешить пользователям с телефонным подключением обходить "зал ожидания"](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) — это политика для каждого организатора, которая определяет, будут ли пользователи, подключающиеся по телефону, напрямую или в зале ожидания, независимо от параметра автоматически допустить **людей** .</span><span class="sxs-lookup"><span data-stu-id="0487a-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="0487a-115">[Разрешить организаторов переопределять параметры ожидания](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**ожидается в ближайшее время**) — это политика для каждого организатора, которая определяет, может ли организатор собрания переопределять параметры, заданные администратором автоматически, допустить **людей** и **Разрешить подключение по телефонной линии Пользователи могут обходить зал ожидания** при планировании нового собрания.</span><span class="sxs-lookup"><span data-stu-id="0487a-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="0487a-116">**Примечание:** Ознакомьтесь с разделом [Управление политиками собраний в Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , чтобы получить полный обзор политик собраний Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0487a-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
