---
title: Определение активности правила для папки "Входящие" в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779064"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="e864f-102">Определение активности правила для папки "Входящие" в журналах аудита</span><span class="sxs-lookup"><span data-stu-id="e864f-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="e864f-103">Вы можете использовать поиск в журнале аудита в центре безопасности & соответствия требованиям Microsoft 365 для просмотра событий правил папки "Входящие" (создание, изменение и удаление правил для папки "Входящие").</span><span class="sxs-lookup"><span data-stu-id="e864f-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="e864f-104">Войдите в [центр соответствия требованиям & безопасности Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e864f-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e864f-105">Перейдите на страницу **Search**  >  **поиска журнала аудита** поиска.</span><span class="sxs-lookup"><span data-stu-id="e864f-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e864f-106">Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .</span><span class="sxs-lookup"><span data-stu-id="e864f-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="e864f-107">В разделе **действия почтового ящика Exchange**убедитесь, что для поля **действия** задано значение создать, **InboxRule создать/изменить/включить или отключить правило для папки "Входящие"**.</span><span class="sxs-lookup"><span data-stu-id="e864f-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="e864f-108">Нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="e864f-108">Click **Search**.</span></span>

<span data-ttu-id="e864f-109">В списке результатов выберите запись аудита.</span><span class="sxs-lookup"><span data-stu-id="e864f-109">In the results, select an audit record.</span></span> <span data-ttu-id="e864f-110">В всплывающем меню сведения щелкните **Дополнительные сведения**.</span><span class="sxs-lookup"><span data-stu-id="e864f-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e864f-111">Сведения о параметрах правила папки "Входящие" отображаются в поле **Параметры** .</span><span class="sxs-lookup"><span data-stu-id="e864f-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="e864f-112">Дополнительные сведения см. в статье [Определение, создал ли пользователь правило для папки "Входящие"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="e864f-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
