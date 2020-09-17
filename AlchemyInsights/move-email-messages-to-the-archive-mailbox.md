---
title: Перемещение сообщений электронной почты в архивный почтовый ящик
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799793"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="77bfd-102">Перемещение электронной почты в архивный почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="77bfd-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="77bfd-103">Если вы хотите, чтобы мы выполняли автоматические проверки для указанных ниже параметров, нажмите кнопку "назад" <--в верхней части этой страницы, а затем введите адрес электронной почты пользователя, с которым возникают проблемы с перемещением электронной почты в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="77bfd-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="77bfd-104">Убедитесь, что **архивный почтовый ящик** включен.</span><span class="sxs-lookup"><span data-stu-id="77bfd-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="77bfd-105">В противном случае выполните действия, описанные в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , чтобы включить архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="77bfd-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="77bfd-106">Чтобы автоматически архивировать сообщения в архивный почтовый ящик, тег хранения с действием **переместить в архив** должен **автоматически применять ко всему тегу почтового ящика (по умолчанию)**.</span><span class="sxs-lookup"><span data-stu-id="77bfd-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="77bfd-107">Выполните действия, описанные в этой статье, чтобы создать тег: [Archive Default Tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="77bfd-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="77bfd-108">Затем добавьте тег **Archive** в политику хранения.</span><span class="sxs-lookup"><span data-stu-id="77bfd-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="77bfd-109">В центре администрирования Exchange выберите **политики хранения** > добавить **тег "переместить в архив** " в политику > **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="77bfd-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="77bfd-110">Теперь [назначьте политику хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для почтового ящика определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="77bfd-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="77bfd-111">Та же политика будет применяться и к **основному** , и к **архивному** почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="77bfd-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="77bfd-112">Может потребоваться принудительно запустить помощник по обслуживанию управляемых папок (MFA) и применить новые параметры к почтовому ящику пользователя.</span><span class="sxs-lookup"><span data-stu-id="77bfd-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="77bfd-113">Выполните следующую команду при [подключении к EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) для запуска помощника по работе с управляемыми папками для определенного почтового ящика:</span><span class="sxs-lookup"><span data-stu-id="77bfd-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="77bfd-114">Start — ManagedFolderAssistant — Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="77bfd-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="77bfd-115">Дополнительные сведения о настройке политики архивации можно найти в разделе [Настройка политики архивации и удаления для почтовых ящиков](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="77bfd-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  