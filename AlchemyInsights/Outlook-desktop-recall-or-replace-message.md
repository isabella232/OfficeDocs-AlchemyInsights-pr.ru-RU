---
title: Настольный отзыв или замена сообщения электронной почты на рабочем столе Outlook
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496124"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="7a142-102">Отзыв или замена сообщения электронной почты в Outlook</span><span class="sxs-lookup"><span data-stu-id="7a142-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="7a142-103">Администратор может **отозвать сообщения от имени пользователей с помощью PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="7a142-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7a142-104">Вы не можете отозвать сообщения из центра администрирования.</span><span class="sxs-lookup"><span data-stu-id="7a142-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7a142-105">Вы можете **отозвать только те сообщения, которые отправляются пользователям в вашей организации**.</span><span class="sxs-lookup"><span data-stu-id="7a142-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7a142-106">Например, если сообщение было отправлено на адрес Gmail, его невозможно отозвать.</span><span class="sxs-lookup"><span data-stu-id="7a142-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7a142-107">Вы можете **отозвать сообщения, отправленные из Outlook 2016 на компьютер**.</span><span class="sxs-lookup"><span data-stu-id="7a142-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7a142-108">Если пользователь отправляет сообщение с помощью Outlook для Mac или Outlook в Интернете, вы не можете отозвать его.</span><span class="sxs-lookup"><span data-stu-id="7a142-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7a142-109">Чтобы отозвать или заменить сообщение электронной почты, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="7a142-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7a142-110">В области папок слева от окна Outlook выберите папку Отправленные.</span><span class="sxs-lookup"><span data-stu-id="7a142-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7a142-111">Дважды щелкните сообщение, которое нужно отозвать, чтобы открыть его.</span><span class="sxs-lookup"><span data-stu-id="7a142-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7a142-112">Перейдите на вкладку **сообщение** , а затем выберите **действия** > **отозвать это сообщение**.</span><span class="sxs-lookup"><span data-stu-id="7a142-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7a142-113">Выберите **Удалить непрочтенные копии этого сообщения** или **Удалить непрочтенные копии и замените на новое сообщение**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="7a142-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7a142-114">Если вы отправляете заменяющее сообщение, создайте сообщение, а затем нажмите кнопку **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="7a142-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7a142-115">Успех или неудача при отзыве сообщения зависит от параметров получателя в Outlook.</span><span class="sxs-lookup"><span data-stu-id="7a142-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7a142-116">Действия, которые необходимо выполнить для проверки отзыва, приведены в [этой статье](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="7a142-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7a142-117">Поиск и удаление сообщений электронной почты в Организации</span><span class="sxs-lookup"><span data-stu-id="7a142-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7a142-118">Если вы не являетесь глобальным администратором, необходимо добавить свою учетную запись в роль диспетчера обнаружения электронных данных или роль управления поиском соответствия требованиям для поиска сообщений.</span><span class="sxs-lookup"><span data-stu-id="7a142-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7a142-119">Чтобы удалить сообщения, необходимо присоединиться к группе ролей Управление организацией или ролью управления поиска и очистки.</span><span class="sxs-lookup"><span data-stu-id="7a142-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7a142-120">Разрешения для этих ролей назначаются в [центре безопасности и соответствия требованиям](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="7a142-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7a142-121">[Создайте поиск контента](https://docs.microsoft.com/office365/securitycompliance/content-search) , чтобы найти сообщение, которое требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="7a142-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7a142-122">[Подключение к PowerShell центра безопасности и соответствия требованиям](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7a142-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7a142-123">Если вы используете многофакторную проверку подлинности, ознакомьтесь со статьей [Подключение к Office 365 Security and Security Center PowerShell с использованием многофакторной проверки подлинности](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7a142-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>