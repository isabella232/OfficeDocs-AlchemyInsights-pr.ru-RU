---
title: Определение активности правила для папки "Входящие" в журналах аудита
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909502"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="98e9d-102">Определение активности правила для папки "Входящие" в журналах аудита</span><span class="sxs-lookup"><span data-stu-id="98e9d-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="98e9d-103">Вы можете использовать поиск в журнале аудита в центре безопасности _Амп_ соответствия требованиям для просмотра событий правил папки "Входящие" (создание, изменение и удаление правил для папки "Входящие").</span><span class="sxs-lookup"><span data-stu-id="98e9d-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="98e9d-104">Вход в [центр соответствия требованиям _Амп_ безопасности Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="98e9d-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="98e9d-105">Щелкните **Поиск и исследование** , а затем выберите **Поиск в журнале аудита**.</span><span class="sxs-lookup"><span data-stu-id="98e9d-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="98e9d-106">Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .</span><span class="sxs-lookup"><span data-stu-id="98e9d-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="98e9d-107">В разделе **действия почтовоГо ящика Exchange**убедитесь, что для поля **действия** задано значение создать, **InboxRule создать/изменить/включить или отключить правило для папки "Входящие"**.</span><span class="sxs-lookup"><span data-stu-id="98e9d-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="98e9d-108">Нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="98e9d-108">Click **Search**.</span></span>

<span data-ttu-id="98e9d-109">В списке результатов выберите запись аудита.</span><span class="sxs-lookup"><span data-stu-id="98e9d-109">In the results, select an audit record.</span></span> <span data-ttu-id="98e9d-110">В всплывающем меню сведения щелкните **Дополнительные сведения**.</span><span class="sxs-lookup"><span data-stu-id="98e9d-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="98e9d-111">Сведения о параметрах правила папки "Входящие" отображаются в поле **Параметры** .</span><span class="sxs-lookup"><span data-stu-id="98e9d-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="98e9d-112">Дополнительные сведения см. в статье [Определение, создал ли пользователь правило для папки "Входящие"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="98e9d-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
