---
title: Определение событий удаления сообщений в журналах аудита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716509"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="d7fe6-102">Журналы аудита для удаленных сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="d7fe6-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="d7fe6-103">Начиная с 2019 января Майкрософт по умолчанию отключается ведение журнала аудита почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="d7fe6-104">В противном случае чтобы просмотреть события удаления сообщений для определенного пользователя, необходимо вручную включить действия Delete для аудита.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="d7fe6-105">Если ведение журнала аудита почтовых ящиков уже включено для вашей организации или для определенного пользователя, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="d7fe6-106">Вход в [центр соответствия требованиям & безопасности Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d7fe6-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d7fe6-107">Щелкните **Поиск и исследование** , а затем выберите **Поиск в журнале аудита**.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="d7fe6-108">Выберите диапазон дат в полях **Дата начала** и **Дата окончания** .</span><span class="sxs-lookup"><span data-stu-id="d7fe6-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d7fe6-109">Укажите имя пользователя для пользователя, которого нужно исследовать (пользователя, который удалил элементы).</span><span class="sxs-lookup"><span data-stu-id="d7fe6-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="d7fe6-110">В поле **действия** выберите пункт **Удаленные сообщения из папки "Удаленные** " и **перемещаете сообщения в папку "Удаленные**".</span><span class="sxs-lookup"><span data-stu-id="d7fe6-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="d7fe6-111">Нажмите кнопку **Поиск**.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-111">Click **Search**.</span></span>

<span data-ttu-id="d7fe6-112">В списке результатов выберите запись аудита.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-112">In the results, select an audit record.</span></span> <span data-ttu-id="d7fe6-113">В всплывающем меню сведения щелкните **Дополнительные сведения**.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d7fe6-114">Дополнительные сведения об удаленном элементе (например, строке темы и расположении элемента при его удалении) отображаются в поле **аффектедитемс** .</span><span class="sxs-lookup"><span data-stu-id="d7fe6-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="d7fe6-115">Свойство **клиентинфостринг** будет отображаться в том случае, если удаление произошло в Outlook, Outlook в Интернете (прежнее название Outlook Web App) или на любом другом устройстве.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="d7fe6-116">Дополнительную информацию можно узнать в статье [Определение того, кто настраивает переадресацию электронной почты для почтового ящика](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="d7fe6-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="d7fe6-117">**Note**: вы не можете получать удаленные элементы с помощью функции журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="d7fe6-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="d7fe6-118">Чтобы получить удаленные сообщения в Outlook в Интернете, ознакомьтесь со статьей [Восстановление удаленных элементов в Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="d7fe6-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
