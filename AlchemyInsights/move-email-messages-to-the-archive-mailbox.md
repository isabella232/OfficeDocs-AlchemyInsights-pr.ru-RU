---
title: Перемещение сообщений электронной почты в архивный почтовый ящик
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511053"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="69a05-102">Перемещение электронной почты в архивный почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="69a05-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="69a05-103">Убедитесь, что **архивный почтовый ящик** включен.</span><span class="sxs-lookup"><span data-stu-id="69a05-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="69a05-104">В противном случае выполните действия, описанные в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , чтобы включить архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="69a05-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="69a05-105">Чтобы автоматически архивировать сообщения в архивный почтовый ящик, тег хранения с действием **переместить в архив** должен **автоматически применять ко всему тегу почтового ящика (по умолчанию)**.</span><span class="sxs-lookup"><span data-stu-id="69a05-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="69a05-106">Выполните действия, описанные в этой статье, чтобы создать тег: [Archive Default Tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="69a05-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="69a05-107">Затем добавьте тег **Archive** в политику хранения.</span><span class="sxs-lookup"><span data-stu-id="69a05-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="69a05-108">В центре администрирования Exchange выберите **политики хранения** > добавить **тег "переместить в архив** " в политику > **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="69a05-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="69a05-109">Теперь [назначьте политику хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для почтового ящика определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="69a05-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="69a05-110">Та же политика будет применяться и к **основному** , и к **архивному** почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="69a05-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="69a05-111">Может потребоваться принудительно запустить помощник по обслуживанию управляемых папок (MFA) и применить новые параметры к почтовому ящику пользователя.</span><span class="sxs-lookup"><span data-stu-id="69a05-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="69a05-112">Выполните следующую команду при [подключении к EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) для запуска помощника по работе с управляемыми папками для определенного почтового ящика:</span><span class="sxs-lookup"><span data-stu-id="69a05-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="69a05-113">Start — ManagedFolderAssistant — Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="69a05-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="69a05-114">Дополнительные сведения о настройке политики архивации можно найти в разделе [Настройка политики архивации и удаления для почтовых ящиков](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="69a05-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  