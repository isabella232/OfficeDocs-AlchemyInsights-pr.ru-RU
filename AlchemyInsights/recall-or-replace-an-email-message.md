---
title: Отзыв или замена сообщения электронной почты
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353519"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="9bd45-102">Отзыв или замена сообщения электронной почты в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9bd45-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="9bd45-103">Вы можете **отозвать только те сообщения, которые отправляются пользователям в вашей организации**.</span><span class="sxs-lookup"><span data-stu-id="9bd45-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="9bd45-104">Например, если сообщение было отправлено на адрес Gmail, его невозможно отозвать.</span><span class="sxs-lookup"><span data-stu-id="9bd45-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="9bd45-105">Вы можете **отозвать сообщения, отправленные из Outlook для компьютера**.</span><span class="sxs-lookup"><span data-stu-id="9bd45-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="9bd45-106">Если пользователь отправляет сообщение с помощью Outlook для Mac или Outlook в Интернете, вы не можете отозвать его.</span><span class="sxs-lookup"><span data-stu-id="9bd45-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="9bd45-107">Администратор клиента может **отзывать сообщения от имени пользователей с помощью PowerShell** (Дополнительные сведения см. в разделе [Поиск и удаление сообщений электронной почты](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="9bd45-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="9bd45-108">Вы не можете отозвать сообщения из центра администрирования.</span><span class="sxs-lookup"><span data-stu-id="9bd45-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="9bd45-109">Прокрутите список вниз до раздела "Поиск и удаление сообщений электронной почты в вашей организации" для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="9bd45-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="9bd45-110">**Отзыв или замена отправленного сообщения электронной почты**</span><span class="sxs-lookup"><span data-stu-id="9bd45-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="9bd45-111">В области папок слева от окна Outlook выберите папку Отправленные.</span><span class="sxs-lookup"><span data-stu-id="9bd45-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="9bd45-112">Откройте сообщение, которое нужно отозвать.</span><span class="sxs-lookup"><span data-stu-id="9bd45-112">Open the message that you want to recall.</span></span> <span data-ttu-id="9bd45-113">Необходимо дважды щелкнуть, чтобы открыть сообщение.</span><span class="sxs-lookup"><span data-stu-id="9bd45-113">You must double-click to open the message.</span></span> <span data-ttu-id="9bd45-114">Если вы выберете сообщение, которое появится в области чтения, вы не сможете отозвать сообщение.</span><span class="sxs-lookup"><span data-stu-id="9bd45-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="9bd45-115">На вкладке Сообщение выберите **действия**  >  **отозвать это сообщение**.</span><span class="sxs-lookup"><span data-stu-id="9bd45-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="9bd45-116">Выберите команду **Удалить непрочтенные копии этого сообщения** или **Удалить непрочтенные копии и замените на новое сообщение**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="9bd45-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="9bd45-117">Если вы отправляете заменяющее сообщение, создайте сообщение, а затем нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="9bd45-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="9bd45-118">Успех или неудача при отзыве сообщения зависит от параметров получателей в Outlook.</span><span class="sxs-lookup"><span data-stu-id="9bd45-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="9bd45-119">Дополнительные сведения о том, как проверить отзыв, можно найти в статье [отзыв или замена отправленного сообщения электронной почты](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="9bd45-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="9bd45-120">**_Для поиска и удаления сообщений электронной почты в Организации_** проще всего сделать глобальным администратором. Если вы не являетесь глобальным администратором, необходимо добавить свою учетную запись в группу ролей диспетчера eDiscovery или в роль управления поиском соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="9bd45-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="9bd45-121">Чтобы удалить сообщения, необходимо присоединиться к группе ролей Управление организацией или ролью управления поиска и очистки.</span><span class="sxs-lookup"><span data-stu-id="9bd45-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="9bd45-122">Разрешения для этих ролей назначаются в [центре безопасности & соответствия требованиям](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9bd45-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="9bd45-123">[Создайте поиск контента](https://docs.microsoft.com/microsoft-365/compliance/content-search) , чтобы найти сообщение, которое требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="9bd45-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="9bd45-124">[Подключение к Центру безопасности и соответствия требованиям Windows PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9bd45-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="9bd45-125">Если вы используете MFA (многофакторную проверку подлинности), ознакомьтесь со статьей [Подключение к Microsoft 365 Security &s PowerShell центра соответствия требованиям с использованием многофакторной проверки подлинности](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9bd45-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
