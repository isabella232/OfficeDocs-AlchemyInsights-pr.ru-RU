---
title: Поиск IP-адреса в журнале аудита
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465004"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="6804c-102">Поиск IP-адреса в журнале аудита</span><span class="sxs-lookup"><span data-stu-id="6804c-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="6804c-103">IP-адрес, соответствующий действию пользователя или администратора, отображается в журналах аудита.</span><span class="sxs-lookup"><span data-stu-id="6804c-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="6804c-104">Сведения о клиентах также регистрируются.</span><span class="sxs-lookup"><span data-stu-id="6804c-104">The client information is also logged.</span></span> <span data-ttu-id="6804c-105">Вот как определить IP-адрес:</span><span class="sxs-lookup"><span data-stu-id="6804c-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="6804c-106">Перейдите в Центр безопасности [Office 365 & соответствия](https://go.microsoft.com/fwlink/p/?linkid=2077143)требованиям.</span><span class="sxs-lookup"><span data-stu-id="6804c-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="6804c-107">Выберите **поиск**  >  **[журнала аудита поиска.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="6804c-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="6804c-108">Если вы видите уведомление о необходимости включить аудит, включаем его сейчас.</span><span class="sxs-lookup"><span data-stu-id="6804c-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="6804c-109">Если эта функция не включена, результаты поиска не смогут извлекать данные из предыдущих дат.</span><span class="sxs-lookup"><span data-stu-id="6804c-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="6804c-110">Если вас интересует определенное действие, выберите его из списка **Действия;** в противном случае по умолчанию все действия будут возвращены выбранному пользователю.</span><span class="sxs-lookup"><span data-stu-id="6804c-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="6804c-111">Обратите внимание, что некоторые действия могут быть недоступны для выбора из меню **Действия;** Однако эти элементы аудита будут возвращены, если **выбраны результаты Show** для всех действий (параметр по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="6804c-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="6804c-112">Укажите диапазон дат, а в поле **Пользователи** выберите имя пользователя для пользователя, который необходимо исследовать.</span><span class="sxs-lookup"><span data-stu-id="6804c-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="6804c-113">Выберите **поиск**.</span><span class="sxs-lookup"><span data-stu-id="6804c-113">Select **Search**.</span></span> <span data-ttu-id="6804c-114">Действия отображаются в **статье Результаты**.</span><span class="sxs-lookup"><span data-stu-id="6804c-114">The activities appear under **Results**.</span></span> <span data-ttu-id="6804c-115">Вы можете увидеть IP-адрес для каждого действия.</span><span class="sxs-lookup"><span data-stu-id="6804c-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="6804c-116">Чтобы просмотреть сведения, выберите действие и выберите **дополнительные сведения.**</span><span class="sxs-lookup"><span data-stu-id="6804c-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="6804c-117">Дополнительные данные см. в журнале [аудита Office 365, чтобы устранить распространенные сценарии.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="6804c-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>