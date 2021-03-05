---
title: Узнайте, кто настроил пересылку в почтовом ящике и как
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464871"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="b97e2-102">Узнайте, кто настроил пересылку в почтовом ящике и как</span><span class="sxs-lookup"><span data-stu-id="b97e2-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="b97e2-103">Если на почтовом ящике была задана внешняя пересылаемая пересылаемая почта, эта деятельность проводится аудит в Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="b97e2-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="b97e2-104">Вот как найти действия в журнале аудита:</span><span class="sxs-lookup"><span data-stu-id="b97e2-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="b97e2-105">Перейдите в Центр безопасности [Office 365 & соответствия](https://go.microsoft.com/fwlink/p/?linkid=2077143)требованиям.</span><span class="sxs-lookup"><span data-stu-id="b97e2-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b97e2-106">Выберите **поиск** >  **журнала аудита поиска.**</span><span class="sxs-lookup"><span data-stu-id="b97e2-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b97e2-107">Если вы видите уведомление о необходимости включить аудит, включаем его сейчас.</span><span class="sxs-lookup"><span data-stu-id="b97e2-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="b97e2-108">Если эта функция не включена, результаты поиска не смогут извлекать данные из предыдущих дат.</span><span class="sxs-lookup"><span data-stu-id="b97e2-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b97e2-109">Убедитесь, **что поле Действия** настроено для показа **результатов для всех действий** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="b97e2-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="b97e2-110">Укажите диапазон дат.</span><span class="sxs-lookup"><span data-stu-id="b97e2-110">Specify the date range.</span></span> <span data-ttu-id="b97e2-111">Не нужно указывать имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b97e2-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="b97e2-112">Выберите **поиск**.</span><span class="sxs-lookup"><span data-stu-id="b97e2-112">Select **Search**.</span></span> <span data-ttu-id="b97e2-113">Действия отображаются в **статье Результаты**.</span><span class="sxs-lookup"><span data-stu-id="b97e2-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="b97e2-114">Выберите **результаты фильтрации,** а затем введите **набор почтовых ящиков** в поле **фильтра Действия.**</span><span class="sxs-lookup"><span data-stu-id="b97e2-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="b97e2-115">Это возвращает все **действия Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="b97e2-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="b97e2-116">Чтобы просмотреть сведения, выберите действие, а затем выберите **дополнительные сведения.**</span><span class="sxs-lookup"><span data-stu-id="b97e2-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="b97e2-117">В **статье Параметры** можно увидеть адрес электронной почты, заданный в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b97e2-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="b97e2-118">**UserID представляет** пользователя, настроившего внешнюю пересылку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b97e2-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="b97e2-119">Дополнительные данные см. в [журнале аудита Office 365, чтобы устранить распространенные сценарии.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="b97e2-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>