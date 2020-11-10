---
title: Использование стикерами в беседах в Teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947513"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="dbcc4-102">Использование стикерами в беседах в Teams</span><span class="sxs-lookup"><span data-stu-id="dbcc4-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="dbcc4-103">Стикерами доступ в чате в Teams включен по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dbcc4-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="dbcc4-104">Как администратор вы можете контролировать доступность стикерами для пользователей, [настроив политику обмена сообщениями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) и убедившись в **том, что** **Использование стикерами в беседах** включено.</span><span class="sxs-lookup"><span data-stu-id="dbcc4-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="dbcc4-105">Если GIF в беседах Teams не работает должным образом, убедитесь, что:</span><span class="sxs-lookup"><span data-stu-id="dbcc4-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="dbcc4-106">[Политика обмена сообщениями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) должна разрешить стикерами.</span><span class="sxs-lookup"><span data-stu-id="dbcc4-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="dbcc4-107">Чтобы проверить с помощью командлетов PowerShell, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="dbcc4-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="dbcc4-108">Убедитесь, что вы можете [управлять Teams с помощью PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="dbcc4-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="dbcc4-109">Выполните команду PowerShell [Get-кстеамсмессагингполици-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и убедитесь, что для **Алловгифи** задано **значение true**.</span><span class="sxs-lookup"><span data-stu-id="dbcc4-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="dbcc4-110">Если для **алловгифи** задано **значение false** , выполните следующую команду PowerShell [Set-Кстеамсмессагингполици-Identity global-алловгифи $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="dbcc4-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="dbcc4-111">Для предоставления доступа к URL-адресу Giphy необходимо включить [необязательный подключенный интерфейс](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="dbcc4-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="dbcc4-112">Если для клиента настроено несколько политик обмена сообщениями Teams, можно определить удостоверение политики, назначенной для затронутого пользователя, с помощью команды PowerShell [Get – CsOnlineUser – Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Выберите Теамсмессагингполици.</span><span class="sxs-lookup"><span data-stu-id="dbcc4-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
