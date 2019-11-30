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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626361"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Управление параметрами и уровнем участия в зале ожидания

Если вы хотите разрешить всем пользователям, в том числе пользователям с телефонным подключением, внешним и анонимным пользователям обходить себя в Microsoft Teams, вы можете использовать PowerShell. Ниже приведен пример изменения глобальной политики собраний для Организации.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Для этого командлета в настоящее время требуется использование модуля PowerShell Skype для бизнеса. Чтобы запустить программу установки для использования этого командлета, изучите [Управление политиками с помощью PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Можно настроить новую политику, которая затем потребуется применить к пользователям. Если вы измените глобальную политику, она будет автоматически применена к пользователям. При изменении политики необходимо подождать не менее 4 часов и до 24 часов, чтобы политики вступили в силу.

Прежде чем вносить эти изменения, ознакомьтесь с приведенной ниже документацией, чтобы убедиться в том, что это позволяет.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Общие сведения об элементах управления политикой для собраний в Teams

- [Автоматически](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) допустить люди — это политика для каждого организатора, которая определяет, присоединяет ли люди непосредственно или ждет, пока пользователь не пройдет проверку подлинности.

- [Разрешить анонимным пользователям начинать собрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) — это политика организатора, которая определяет, могут ли анонимные пользователи, включая B2B и Федеративные пользователи, присоединиться к собранию пользователя без прошедшего проверку подлинности пользователя из Организации в присутствии.

- [Разрешить пользователям с телефонным подключением обходить "зал ожидания"](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) — это политика для каждого организатора, которая определяет, будут ли пользователи, подключающиеся по телефону, напрямую или в зале ожидания, независимо от параметра автоматически допустить **людей** .

- [Разрешить организаторов переопределять параметры ожидания](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**ожидается**) — это политика для каждого организатора, которая определяет, может ли организатор собрания переопределять параметры, заданные администратором **автоматически** , допустить людей и **разрешать пользователям с телефонным подключением обходить** свое время ожидания при планировании нового собрания.

**Примечание:** Ознакомьтесь с разделом [Управление политиками собраний в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , чтобы получить полный обзор политик собраний Microsoft Teams.
