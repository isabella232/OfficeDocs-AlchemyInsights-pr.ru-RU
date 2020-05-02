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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="ee5b0-102">Частные каналы в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ee5b0-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="ee5b0-103">Частные каналы — это новая функция Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ee5b0-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="ee5b0-104">Обратите внимание, что частные каналы не могут быть преобразованы из стандартных каналов и наоборот.</span><span class="sxs-lookup"><span data-stu-id="ee5b0-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="ee5b0-105">Для получения дополнительных сведений о частных каналах, таких как сведения о [создании и членстве на частных каналах](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) и [сайтах личных сайтов SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), ознакомьтесь со статьей [частные каналы в Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="ee5b0-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="ee5b0-106">**Примечание:** Так как конфигурация хранения сообщений частных каналов пока не поддерживается, то для клиентов, для которых включена политика хранения, частные каналы по умолчанию отключены.</span><span class="sxs-lookup"><span data-stu-id="ee5b0-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="ee5b0-107">В центре администрирования Teams можно включить частные каналы.</span><span class="sxs-lookup"><span data-stu-id="ee5b0-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="ee5b0-108">Кроме того, обратите внимание, что при хранении сообщений закрытого канала поддерживается хранение файлов, совместно используемых в частных каналах.</span><span class="sxs-lookup"><span data-stu-id="ee5b0-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="ee5b0-109">**Нужен новый владелец группы?**</span><span class="sxs-lookup"><span data-stu-id="ee5b0-109">**Need a new team owner?**</span></span>

<span data-ttu-id="ee5b0-110">Если владелец личного канала оставляется, вы можете добавить нового владельца команды с помощью Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee5b0-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="ee5b0-111">Чтобы установить PowerShell Teams, перейдите по [адресу](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) .</span><span class="sxs-lookup"><span data-stu-id="ee5b0-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="ee5b0-112">Вот командлет, который потребуется:</span><span class="sxs-lookup"><span data-stu-id="ee5b0-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="ee5b0-113">Более подробную информацию о Teams PowerShell можно узнать в статье [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ee5b0-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
