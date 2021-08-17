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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059609"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Управление настройками лобби и уровнем участия в Teams

Если вы хотите разрешить всем пользователям, включая пользователей dial-in, внешних и анонимных, обходить **лобби,** используйте PowerShell для выполнения этой задачи. Вот пример изменения глобальной политики собраний для организации.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Этот командлет в настоящее время требует использования Skype для бизнеса PowerShell. Чтобы настроиться на использование этого комлета, ознакомьтесь с политиками [управления с помощью PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

После того как вы настроили политику, ее необходимо применить к пользователям; или, если вы изменили глобальную политику, она будет автоматически применяться к пользователям. Для любых изменений политики необходимо подождать не менее 4 часов до **24** часов, чтобы политики вступили в силу. 

Не забудьте просмотреть ниже документацию, прежде чем вносить эти изменения, чтобы точно понять, что это позволяет.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Понимание Teams элементов управления политикой лоббирования собраний

Эти параметры контролируют, какие участники собраний ждут в вестибюле, прежде чем они будут допущены к собранию, и уровень участия в собрании. Вы можете использовать PowerShell для обновления параметров политики собраний, которые еще не реализованы (помечены как "скоро") в центре администрирования Teams. См. ниже, например, cmdlet PowerShell, который позволяет всем пользователям обходить вестибюль.

- [Автоматически допускается, что](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) люди являются политикой, которая контролирует, присоединяются ли люди к собранию напрямую или ждут в вестибюле, пока они не будут допущены пользователем с проверкой подлинности.

- [Разрешить](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) анонимным людям начинать собрание — это политика для каждого организатора, которая контролирует, могут ли анонимные люди, включая B2B и федерабельных пользователей, присоединяться к собранию пользователя без проверки подлинности пользователя из организации, которая присутствовала на собрании.

- [Разрешить](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) пользователям набора номеров обход вестибюля **(в** ближайшее время) — это политика для каждого организатора, которая  контролирует, присоединяются ли люди, которые звонят по телефону, непосредственно к собранию или ждут в вестибюле независимо от параметра автоматически допуска людей.

- Разрешить организаторам переопределять параметры лобби (в ближайшее **время)**— это политика для каждого организатора,  которая контролирует,  может ли организатор собрания переопределять параметры лобби, установленные администратором в Автоматическом впуске людей, и разрешить пользователям в диалоговом режиме обход вестибюля при запланировании нового собрания. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)

**Примечание:** Ознакомьтесь [с политиками управления собраниями в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) для полного Microsoft Teams политик собраний.
