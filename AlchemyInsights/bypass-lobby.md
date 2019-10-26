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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37654269"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Управление параметрами и уровнем участия в зале ожидания

Если вы хотите разрешить всем пользователям, в том числе пользователям с телефонным подключением, внешним пользователям и анонимным пользователям обходить свое время ожидания, вы можете использовать PowerShell. Ниже приведен пример изменения глобальной политики собраний для Организации.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Для этого командлета в настоящее время требуется использование модуля PowerShell Skype для бизнеса. Чтобы запустить программу установки для использования этого командлета, изучите [Управление политиками с помощью PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Можно настроить новую политику, которая затем потребуется применить к пользователям. Если вы измените глобальную политику, она будет автоматически применена к пользователям. При изменении политики необходимо подождать не менее 4 часов и до 24 часов, чтобы политики вступили в силу.

Прежде чем вносить эти изменения, ознакомьтесь с приведенной ниже документацией, чтобы убедиться в том, что это позволяет.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Общие сведения об элементах управления политикой для собраний в Teams

- [Автоматически](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) допустить люди — это политика для каждого организатора, которая определяет, присоединяет ли люди непосредственно или ждет, пока пользователь не пройдет проверку подлинности.

- [Разрешить анонимным пользователям начинать собрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) — это политика организатора, которая определяет, могут ли анонимные пользователи, включая B2B и Федеративные пользователи, присоединиться к собранию пользователя без прошедшего проверку подлинности пользователя из Организации в присутствии.

- [Разрешить пользователям с телефонным подключением обходить "зал ожидания"](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) — это политика для каждого организатора, которая определяет, будут ли пользователи, подключающиеся по телефону, напрямую или в зале ожидания, независимо от параметра автоматически допустить **людей** .

- [Разрешить организаторов переопределять параметры ожидания](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**ожидается в ближайшее время**) — это политика для каждого организатора, которая определяет, может ли организатор собрания переопределять параметры, заданные администратором автоматически, допустить **людей** и **Разрешить подключение по телефонной линии Пользователи могут обходить зал ожидания** при планировании нового собрания.

**Примечание:** Ознакомьтесь с разделом [Управление политиками собраний в Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , чтобы получить полный обзор политик собраний Microsoft Teams.
