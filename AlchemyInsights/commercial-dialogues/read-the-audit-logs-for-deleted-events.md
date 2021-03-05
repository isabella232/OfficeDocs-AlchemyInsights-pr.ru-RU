---
title: Чтение журналов аудита для удаленных событий
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464859"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="a7255-102">Чтение журналов аудита для удаленных событий</span><span class="sxs-lookup"><span data-stu-id="a7255-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="a7255-103">Вот как это сделать:</span><span class="sxs-lookup"><span data-stu-id="a7255-103">Here's how to do this:</span></span>

1. <span data-ttu-id="a7255-104">Перейдите в Центр безопасности [Office 365 & соответствия](https://go.microsoft.com/fwlink/p/?linkid=2077143)требованиям.</span><span class="sxs-lookup"><span data-stu-id="a7255-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="a7255-105">Выберите **поиск**  >  [**журнала аудита поиска.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="a7255-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="a7255-106">Если вы видите уведомление о необходимости включить функцию, включаем ее и включаем.</span><span class="sxs-lookup"><span data-stu-id="a7255-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="a7255-107">Если функция не включена, результаты поиска не смогут извлекать данные из предыдущих дат.</span><span class="sxs-lookup"><span data-stu-id="a7255-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="a7255-108">Выберите **Действия,** а затем найдите **действия почтовых ящиков Exchange.**</span><span class="sxs-lookup"><span data-stu-id="a7255-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="a7255-109">Выберите **удаленные сообщения из папки "Удаленные** элементы" и "Перенесенные" сообщения в **параметры папки "Удаленные** элементы".</span><span class="sxs-lookup"><span data-stu-id="a7255-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="a7255-110">После этого щелкните за пределами области, чтобы свести к минимуму области **Действия.**</span><span class="sxs-lookup"><span data-stu-id="a7255-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="a7255-111">Укажите диапазон дат, а затем в поле **Пользователи** выберите имя пользователя для пользователя, который необходимо исследовать.</span><span class="sxs-lookup"><span data-stu-id="a7255-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="a7255-112">Вы можете выбрать несколько пользователей одновременно.</span><span class="sxs-lookup"><span data-stu-id="a7255-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="a7255-113">Выберите **поиск**.</span><span class="sxs-lookup"><span data-stu-id="a7255-113">Select **Search**.</span></span> <span data-ttu-id="a7255-114">Действия отображаются в **статье Результаты**.</span><span class="sxs-lookup"><span data-stu-id="a7255-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="a7255-115">Чтобы просмотреть сведения, выберите действие, а затем выберите **дополнительные сведения.**</span><span class="sxs-lookup"><span data-stu-id="a7255-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="a7255-116">Дополнительные сведения об удалении элемента, например о строке субъекта и расположении элемента при его удалении, отображаются в **поле AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="a7255-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="a7255-117">Вы не можете восстановить удаленные элементы с помощью функции журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="a7255-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="a7255-118">Чтобы восстановить удаленные элементы, см. в статьи Восстановление удаленных элементов или [электронную почту в Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="a7255-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="a7255-119">Дополнительные данные см. в [журнале аудита Office 365, чтобы устранить распространенные сценарии.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="a7255-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
