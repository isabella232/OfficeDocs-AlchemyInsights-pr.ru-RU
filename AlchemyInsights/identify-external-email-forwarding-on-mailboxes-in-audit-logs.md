---
title: Определение внешних переадресации электронной почты в почтовых ящиках в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716473"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c0d9d-102">Определение времени настройки переадресации внешней почты для почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="c0d9d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c0d9d-103">Когда пользователь Microsoft 365 настраивает внешнюю переадресацию электронной почты в почтовом ящике, действие подлежит аудиту в рамках командлета **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="c0d9d-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c0d9d-104">Вы можете просмотреть действие с помощью функции поиска в журнале аудита в центре безопасности & соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c0d9d-105">Войдите в [центр соответствия требованиям & безопасности Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c0d9d-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c0d9d-106">Перейдите на страницу **Search** > **поиска журнала аудита** поиска.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c0d9d-107">Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .</span><span class="sxs-lookup"><span data-stu-id="c0d9d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c0d9d-108">Указывать имя пользователя не требуется.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-108">You don't need to specify a username.</span></span> <span data-ttu-id="c0d9d-109">Убедитесь, что в поле **действия** задано значение **Показать результаты для всех действий**.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c0d9d-110">Нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-110">Click **Search**.</span></span>

<span data-ttu-id="c0d9d-111">В списке результатов щелкните **фильтровать результаты** и введите **Set — Mailbox** в поле фильтр действий.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c0d9d-112">Выберите запись аудита в списке результатов.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-112">Select an audit record in the results.</span></span> <span data-ttu-id="c0d9d-113">В всплывающем меню **сведения** щелкните **Дополнительные сведения**.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c0d9d-114">Необходимо просмотреть сведения о каждой записи аудита, чтобы определить, связано ли действие с переадресацией электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c0d9d-115">**ObjectID**: значение псевдонима для почтового ящика, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c0d9d-116">**Parameters**: _ForwardingSmtpAddress_ указывает целевой адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c0d9d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c0d9d-117">**UserID**: пользователь, который настроил переадресацию электронной почты для почтового ящика в поле **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="c0d9d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c0d9d-118">Дополнительную информацию можно узнать в статье [Определение того, кто настраивает переадресацию электронной почты для почтового ящика](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c0d9d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
