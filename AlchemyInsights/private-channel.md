---
title: Частный канал
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005451"
---
# <a name="private-channels-in-microsoft-teams"></a>Частные каналы в Microsoft Teams

Частные каналы — это новая функция Microsoft Teams. Обратите внимание, что частные каналы не могут быть преобразованы из стандартных каналов и наоборот.

Для получения дополнительных сведений о частных каналах, таких как сведения о [создании и членстве на частных каналах](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) и [сайтах личных сайтов SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), ознакомьтесь со статьей [частные каналы в Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Примечание:** Так как конфигурация хранения сообщений частных каналов пока не поддерживается, то для клиентов, для которых включена политика хранения, частные каналы по умолчанию отключены. В центре администрирования Teams можно включить частные каналы. Кроме того, обратите внимание, что при хранении сообщений закрытого канала поддерживается хранение файлов, совместно используемых в частных каналах.

**Нужен новый владелец группы?**

Если владелец личного канала оставляется, вы можете добавить нового владельца команды с помощью Teams PowerShell.


- Чтобы установить PowerShell Teams, перейдите по [адресу](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) .

Вот командлет, который потребуется:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Более подробную информацию о Teams PowerShell можно узнать в статье [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
