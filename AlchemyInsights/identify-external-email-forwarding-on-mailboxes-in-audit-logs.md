---
title: Определение внешних переадресации электронной почты в почтовых ящиках в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383110"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="20abe-102">Определение времени настройки переадресации внешней почты для почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="20abe-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="20abe-103">Когда пользователь настраивает внешнюю переадресацию электронной почты для почтового ящика, действие подлежит аудиту в рамках командлета **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="20abe-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="20abe-104">Вы можете просмотреть действие с помощью функции поиска в журнале аудита в центре безопасности & соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="20abe-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="20abe-105">Вход в [центр соответствия требованиям & безопасности Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="20abe-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="20abe-106">Щелкните **Поиск и исследование** , а затем выберите **Поиск в журнале аудита**.</span><span class="sxs-lookup"><span data-stu-id="20abe-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="20abe-107">Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .</span><span class="sxs-lookup"><span data-stu-id="20abe-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="20abe-108">Указывать имя пользователя не требуется.</span><span class="sxs-lookup"><span data-stu-id="20abe-108">You don't need to specify a username.</span></span> <span data-ttu-id="20abe-109">Убедитесь, что в поле **действия** задано значение **Показать результаты для всех действий**.</span><span class="sxs-lookup"><span data-stu-id="20abe-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="20abe-110">Нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="20abe-110">Click **Search**.</span></span>

<span data-ttu-id="20abe-111">В списке результатов щелкните **фильтровать результаты** и введите **Set — Mailbox** в поле фильтр действий.</span><span class="sxs-lookup"><span data-stu-id="20abe-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="20abe-112">Выберите запись аудита в списке результатов.</span><span class="sxs-lookup"><span data-stu-id="20abe-112">Select an audit record in the results.</span></span> <span data-ttu-id="20abe-113">В всплывающем меню **сведения** щелкните **Дополнительные сведения**.</span><span class="sxs-lookup"><span data-stu-id="20abe-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="20abe-114">Необходимо просмотреть сведения о каждой записи аудита, чтобы определить, связано ли действие с переадресацией электронной почты.</span><span class="sxs-lookup"><span data-stu-id="20abe-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="20abe-115">**ObjectID**: значение псевдонима для почтового ящика, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="20abe-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="20abe-116">**Parameters**: _ForwardingSmtpAddress_ указывает целевой адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="20abe-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="20abe-117">**UserID**: пользователь, который настроил переадресацию электронной почты для почтового ящика в поле **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="20abe-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="20abe-118">Дополнительную информацию можно узнать в статье [Определение того, кто настраивает переадресацию электронной почты для почтового ящика](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="20abe-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
