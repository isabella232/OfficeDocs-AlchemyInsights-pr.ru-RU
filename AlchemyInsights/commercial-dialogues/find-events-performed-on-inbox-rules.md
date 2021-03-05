---
title: Поиск событий, выполняемых в правилах "Входящие"
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464999"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="502f5-102">Поиск событий, выполняемых в правилах "Входящие"</span><span class="sxs-lookup"><span data-stu-id="502f5-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="502f5-103">Когда правила входящие создаются, меняются или удаляются, события записывают в журнал аудита.</span><span class="sxs-lookup"><span data-stu-id="502f5-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="502f5-104">Вот как их просмотреть:</span><span class="sxs-lookup"><span data-stu-id="502f5-104">Here's how to review them:</span></span>

1. <span data-ttu-id="502f5-105">Перейдите в Центр безопасности [Office 365 & соответствия](https://go.microsoft.com/fwlink/p/?linkid=2077143)требованиям.</span><span class="sxs-lookup"><span data-stu-id="502f5-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="502f5-106">Выберите поиск > журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="502f5-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="502f5-107">Если вы видите уведомление о необходимости включить аудит, включаем его сейчас.</span><span class="sxs-lookup"><span data-stu-id="502f5-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="502f5-108">Если эта функция не включена, результаты поиска не смогут извлекать данные из предыдущих дат.</span><span class="sxs-lookup"><span data-stu-id="502f5-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="502f5-109">Выберите поле Действия и найдите действия почтовых ящиков Exchange, а затем выберите New-InboxRule создать правило входящие из Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="502f5-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="502f5-110">После этого щелкните за пределами области, чтобы свести к минимуму области Действия.</span><span class="sxs-lookup"><span data-stu-id="502f5-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="502f5-111">Укажите диапазон дат, а затем в поле Пользователи выберите имя пользователя для пользователя, который необходимо исследовать.</span><span class="sxs-lookup"><span data-stu-id="502f5-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="502f5-112">Вы можете выбрать несколько пользователей одновременно.</span><span class="sxs-lookup"><span data-stu-id="502f5-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="502f5-113">Выберите поиск.</span><span class="sxs-lookup"><span data-stu-id="502f5-113">Select Search.</span></span> <span data-ttu-id="502f5-114">Действия отображаются в статье Results.</span><span class="sxs-lookup"><span data-stu-id="502f5-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="502f5-115">Чтобы просмотреть сведения, выберите действие и выберите дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="502f5-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="502f5-116">В разделе Параметры вы можете увидеть имя правила, заданные условия и действия, которые будет принимать правило.</span><span class="sxs-lookup"><span data-stu-id="502f5-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="502f5-117">Дополнительные данные см. в журнале аудита Office 365, чтобы устранить распространенные сценарии.</span><span class="sxs-lookup"><span data-stu-id="502f5-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>