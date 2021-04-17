---
title: Ошибка входа в Teams адресации AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822000"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="0a094-102">Ошибка входа в Teams адресации AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="0a094-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="0a094-103">При входе в Microsoft Teams вы можете получить сообщение об ошибке: **Извините, но у нас возникли проблемы с подписью вас в AADSTS9000411: запрос неправильно отформатирован. Параметр "login_hint" дублируется.**</span><span class="sxs-lookup"><span data-stu-id="0a094-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="0a094-104">Чтобы решить эту проблему, убедитесь, что ваши клиенты Microsoft Teams обновлены.</span><span class="sxs-lookup"><span data-stu-id="0a094-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="0a094-105">Для получения дополнительной информации об обновлении вашего клиента см. [Обновление Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0a094-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="0a094-106">Если по какой-то причине вы не можете обновить свой клиент, выход из него приведет к удалению большинства кэшированных данных.</span><span class="sxs-lookup"><span data-stu-id="0a094-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="0a094-107">Однако, если у вас все еще есть проблемы после выхода/входа из системы, выйдите из Teams и очистите кэш клиента, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="0a094-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="0a094-108">Закройте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0a094-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="0a094-109">Перейдите по адресу:%appdata%\microsoft\teams и удалите все файлы.</span><span class="sxs-lookup"><span data-stu-id="0a094-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="0a094-110">Снова откройте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0a094-110">Reopen Microsoft Teams.</span></span>
