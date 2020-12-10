---
title: Включение поддержки размещенной голосовой почты
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608878"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="27827-102">Включение поддержки размещенной голосовой почты</span><span class="sxs-lookup"><span data-stu-id="27827-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="27827-103">Чтобы включить голосовую почту, для **хостедвоицемаил** необходимо задать значение $true.</span><span class="sxs-lookup"><span data-stu-id="27827-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="27827-104">Свойство **хостедвоицемаил** пользователя, использующего удаленную оболочку POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="27827-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="27827-105">Дополнительные сведения о подключении к RPS приведены в [статье Обзор Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) для получения дополнительных сведений о подключении к RPS.</span><span class="sxs-lookup"><span data-stu-id="27827-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="27827-106">Администратор Teams должен войти в удаленную оболочку PowerShell для Teams.</span><span class="sxs-lookup"><span data-stu-id="27827-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="27827-107">В командной консоли PowerShell администратор Teams может выполнить командлет **Set-csuser user@contoso.com-хостедвоицемаил $true** , в котором находится URI SIP пользователя.</span><span class="sxs-lookup"><span data-stu-id="27827-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="27827-108">Репликация изменений в политиках может занять до 24 часов.</span><span class="sxs-lookup"><span data-stu-id="27827-108">Changes to policies can take up to 24 hours to replicate.</span></span>