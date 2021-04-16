---
title: Произошла ошибка проверки ошибки маркера доступа во время посадки в Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813701"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="abd98-102">Ошибка "Ошибка проверки маркера доступа" во время бортовой обработки Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="abd98-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="abd98-103">Эта ошибка обычно наблюдается при истечении срока действия маркера проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="abd98-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="abd98-104">Обычно обновление страницы обновляет маркер.</span><span class="sxs-lookup"><span data-stu-id="abd98-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="abd98-105">Однако эта проблема может сохраняться, если к учетной записи, используемой для настольной аналитики, применяются какие-либо политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="abd98-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="abd98-106">Вы можете просмотреть журналы Входа Azure AD на портале Azure, чтобы узнать, есть ли сбои входа для учетной записи, используемой для onboarding Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="abd98-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="abd98-107">Дополнительные сведения об условном доступе можно получить на сайте [Plan your Conditional Access deployment.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="abd98-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>