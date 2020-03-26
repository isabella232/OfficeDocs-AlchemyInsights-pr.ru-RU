---
title: Значок календаря не отображается в клиенте Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932196"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="38dda-102">Значок календаря не отображается в клиенте Teams</span><span class="sxs-lookup"><span data-stu-id="38dda-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="38dda-103">Для вкладки «Календарь» в Teams требуется доступ к почтовому ящику Exchange через веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="38dda-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="38dda-104">Почтовый ящик Exchange может быть онлайн или локальным.</span><span class="sxs-lookup"><span data-stu-id="38dda-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="38dda-105">Для пользователей в сети, которые не видят вкладку «Календарь», убедитесь, что они [лицензированы для почтового ящика Exchange Online, и почтовый ящик включен](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="38dda-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="38dda-106">Если у пользователя есть действующий почтовый ящик в Exchange Online, но он по-прежнему не видит вкладку «Календарь», возможно, возникла проблема с сетью.</span><span class="sxs-lookup"><span data-stu-id="38dda-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="38dda-107">Используйте [анализатор удаленного подключения Microsoft ](https://testconnectivity.microsoft.com/)и запустите **тесты подключения веб-служб Microsoft Exchange** для затронутого пользователя.</span><span class="sxs-lookup"><span data-stu-id="38dda-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="38dda-108">Наконец, проверьте [приложение Teams - политики настройки приложения](https://admin.teams.microsoft.com/policies/app-setup), чтобы убедиться, что приложение «Календарь» не было удалено из политики, применяемой к пользователю (скорее всего, **глобальной (по умолчанию для всей организации)**.</span><span class="sxs-lookup"><span data-stu-id="38dda-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="38dda-109">Если ваши пользователи размещены локально, вы должны подтвердить, что ваша гибридная конфигурация исправна.</span><span class="sxs-lookup"><span data-stu-id="38dda-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="38dda-110">Используйте [мастер гибридной конфигурации](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) для устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="38dda-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="38dda-111">Обратите внимание, что [для Teams требуется Exchange 2016 CU3 или выше](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="38dda-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
