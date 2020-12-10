---
title: Строка агента пользователя Microsoft EDGE (Настольный)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49609676"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="5a5ac-102">Строка агента пользователя Microsoft EDGE (Настольный)</span><span class="sxs-lookup"><span data-stu-id="5a5ac-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="5a5ac-103">Строки агента пользователя (UA) можно использовать для определения того, какая версия конкретного браузера используется в определенной операционной системе.</span><span class="sxs-lookup"><span data-stu-id="5a5ac-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="5a5ac-104">Как и в других браузерах, Microsoft Edge включает эти сведения в НТТР-заголовок "User-Agent" при выполнении запроса к сайту.</span><span class="sxs-lookup"><span data-stu-id="5a5ac-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="5a5ac-105">Доступ к сведениям о версии браузера также можно получить с помощью JavaScript, запрашивая значение "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="5a5ac-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="5a5ac-106">Мы рекомендуем веб-разработчикам использовать обнаружение компонентов, когда это возможно, для усовершенствования поддержки кода, сокращения кода фрагилити и устранения риска нарушения кода в случае будущих обновлений строк UA.</span><span class="sxs-lookup"><span data-stu-id="5a5ac-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="5a5ac-107">Дополнительные сведения см. в разделе [строка агента пользователя Microsoft EDGE (Рабочий стол)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="5a5ac-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>