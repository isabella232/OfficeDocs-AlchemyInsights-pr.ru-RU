---
title: Обход "зал ожидания"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684963"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Управление параметрами и уровнем участия в Microsoft Teams

Если вы хотите разрешить всем пользователям, в том числе пользователям с телефонным подключением, внешним пользователям и анонимным пользователям, **обходить**эту задачу с помощью PowerShell, используйте PowerShell. В этом примере показано, как изменить глобальную политику собраний для своей организации.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Для этого командлета в настоящее время требуется использование модуля PowerShell Skype для бизнеса. Чтобы приступить к настройке для использования этого командлета, изучите [Управление политиками с помощью PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

После настройки политики ее необходимо применить к пользователям; Если вы изменили глобальную политику, она будет автоматически применена к пользователям. Для вступления в силу любых изменений политики необходимо подождать не менее **4 часов до 24 часов** , чтобы политики вступили в силу. 

Прежде чем вносить эти изменения, ознакомьтесь с приведенной ниже документацией, чтобы убедиться в том, что это позволяет.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Общие сведения об элементах управления политикой для собраний в Teams

Эти параметры определяют, какие участники собрания ожидают, прежде чем они будут допущены на собрание, и уровень участия, разрешенный им на собрании. Вы можете использовать PowerShell, чтобы обновить параметры политики для собраний, которые еще не были реализованы (помечены в ближайшее время) в центре администрирования Teams. Ниже приведен пример командлета PowerShell, который позволяет всем пользователям обходить "зал ожидания".

- [Автоматически](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) допустить люди — это политика для каждого организатора, которая определяет, присоединяет ли люди непосредственно или ждет, пока пользователь не пройдет проверку подлинности.

- [Разрешить анонимным пользователям начинать собрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) — это политика организатора, которая определяет, могут ли анонимные пользователи, включая B2B и Федеративные пользователи, присоединиться к собранию пользователя без прошедшего проверку подлинности пользователя из Организации в присутствии.

- [Разрешить пользователям с телефонным подключением обходить "зал ожидания"](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) — это политика для каждого организатора, которая определяет, будут ли пользователи, подключающиеся по телефону, напрямую или в зале ожидания, независимо от параметра автоматически допустить **людей** .

- [Разрешить организаторов переопределять параметры ожидания](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**ожидается**) — это политика для каждого организатора, которая определяет, может ли организатор собрания переопределять параметры, заданные администратором **автоматически** , допустить людей и **разрешать пользователям с телефонным подключением обходить** свое время ожидания при планировании нового собрания.

**Примечание:** Ознакомьтесь с разделом [Управление политиками собраний в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , чтобы получить полный обзор политик собраний Microsoft Teams.
