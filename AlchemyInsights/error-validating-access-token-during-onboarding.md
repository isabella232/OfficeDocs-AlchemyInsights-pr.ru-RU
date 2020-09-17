---
title: Ошибка при проверке маркера доступа во время выполнения анализа настольных систем
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783564"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="444be-102">Ошибка "ошибка при проверке маркера доступа" во время входящей миграции настольных систем</span><span class="sxs-lookup"><span data-stu-id="444be-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="444be-103">Эта ошибка обычно наблюдается, когда истечет срок действия маркера проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="444be-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="444be-104">Как правило, обновление страницы обновляет токен.</span><span class="sxs-lookup"><span data-stu-id="444be-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="444be-105">Однако эта проблема может быть недоступна, если к учетной записи, используемой для аналитики на системной плате, применяются какие политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="444be-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="444be-106">Вы можете просмотреть журналы входа Azure AD на портале Azure, чтобы проверить наличие неудачных попыток входа для учетной записи, используемой для входящей миграции настольных систем.</span><span class="sxs-lookup"><span data-stu-id="444be-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="444be-107">Для получения дополнительных сведений о условном доступе перейдите [в план развертывания условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="444be-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>