---
title: Определение событий удаления сообщений в журналах аудита
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416722"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="9017e-102">Журналы аудита для удаленных сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="9017e-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="9017e-103">Начиная с 2019 января Майкрософт по умолчанию отключается ведение журнала аудита почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="9017e-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="9017e-104">В противном случае чтобы просмотреть события удаления сообщений для определенного пользователя, необходимо вручную включить действия Delete для аудита.</span><span class="sxs-lookup"><span data-stu-id="9017e-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="9017e-105">Если ведение журнала аудита почтовых ящиков уже включено для вашей организации или для определенного пользователя, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="9017e-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="9017e-106">Вход в [центр соответствия требованиям _Амп_ безопасности Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9017e-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="9017e-107">Щелкните **Поиск и исследование** , а затем выберите **Поиск в журнале аудита**.</span><span class="sxs-lookup"><span data-stu-id="9017e-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="9017e-108">Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .</span><span class="sxs-lookup"><span data-stu-id="9017e-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9017e-109">Укажите имя пользователя для пользователя, которого нужно исследовать (пользователя, который удалил элементы).</span><span class="sxs-lookup"><span data-stu-id="9017e-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="9017e-110">В поле **действия** выберите пункт **Удаленные сообщения из папки "Удаленные** " и **перемещаете сообщения в папку "Удаленные**".</span><span class="sxs-lookup"><span data-stu-id="9017e-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="9017e-111">Нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="9017e-111">Click **Search**.</span></span>

<span data-ttu-id="9017e-112">В списке результатов выберите запись аудита.</span><span class="sxs-lookup"><span data-stu-id="9017e-112">In the results, select an audit record.</span></span> <span data-ttu-id="9017e-113">В всплывающем меню сведения щелкните **Дополнительные сведения**.</span><span class="sxs-lookup"><span data-stu-id="9017e-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9017e-114">Дополнительные сведения об удаленном элементе (например, строке темы и расположении элемента при его удалении) отображаются в поле **аффектедитемс** .</span><span class="sxs-lookup"><span data-stu-id="9017e-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="9017e-115">Свойство **клиентинфостринг** будет отображаться в том случае, если удаление произошло в Outlook, Outlook в Интернете (прежнее название Outlook Web App) или на любом другом устройстве.</span><span class="sxs-lookup"><span data-stu-id="9017e-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="9017e-116">Дополнительную информацию можно узнать в статье [Определение того, кто настраивает переадресацию электронной почты для почтового ящика](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="9017e-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="9017e-117">**Note**: вы не можете получать удаленные элементы с помощью функции журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="9017e-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="9017e-118">Чтобы получить удаленные сообщения в Outlook в Интернете, ознакомьтесь со статьей [Восстановление удаленных элементов в Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="9017e-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
