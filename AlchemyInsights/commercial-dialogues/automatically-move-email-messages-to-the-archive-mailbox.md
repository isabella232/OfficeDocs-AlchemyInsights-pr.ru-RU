---
title: Автоматически перемещение сообщений электронной почты в почтовый ящик архива
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737586"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="c01a3-102">Автоматически перемещение сообщений электронной почты в почтовый ящик архива</span><span class="sxs-lookup"><span data-stu-id="c01a3-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="c01a3-103">Ниже понастройка политики автоматического перемещения старой электронной почты пользователя в архивный почтовый ящик:</span><span class="sxs-lookup"><span data-stu-id="c01a3-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="c01a3-104">Перейдите & [**в архив**](https://go.microsoft.com/fwlink/p/?linkid=2077143)управления данными по обеспечению соответствия требованиям, чтобы проверить, включен ли для пользователя  >    >   архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="c01a3-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="c01a3-105">Если этого не было, нажмите **кнопку Включить** затем **Да** в поле предупреждения.</span><span class="sxs-lookup"><span data-stu-id="c01a3-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="c01a3-106">Перейдите [**в центр администрирования Exchange > управления > хранения.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="c01a3-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="c01a3-107">Выберите значок +, а **затем выберите автоматически примениться к всему почтовому ящику.**</span><span class="sxs-lookup"><span data-stu-id="c01a3-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="c01a3-108">Назначьте имя тегу хранения и выберите **Move to Archive**.</span><span class="sxs-lookup"><span data-stu-id="c01a3-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="c01a3-109">В течение периода хранения введите необходимое время, например 90 дней.</span><span class="sxs-lookup"><span data-stu-id="c01a3-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="c01a3-110">Щелкните **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c01a3-110">Click **Save**.</span></span>
5. <span data-ttu-id="c01a3-111">Теперь создайте политику хранения: выберите **политики хранения,** выберите значок, чтобы добавить новую политику.</span><span class="sxs-lookup"><span data-stu-id="c01a3-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="c01a3-112">Назначьте имя политике хранения, нажмите кнопку и прокрутите, чтобы найти и добавить только что созданный тег хранения.</span><span class="sxs-lookup"><span data-stu-id="c01a3-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="c01a3-113">Щелкните **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c01a3-113">Click **Save**.</span></span>
7. <span data-ttu-id="c01a3-114">Наконец, применить политику хранения к почтовому ящику пользователя: все еще в центре администрирования Exchange перейдите к почтовым  >  **ящикам получателей.**</span><span class="sxs-lookup"><span data-stu-id="c01a3-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="c01a3-115">Выберите всех пользователей, к которым необходимо применить политику, а затем выберите **Edit** (значок карандаша).</span><span class="sxs-lookup"><span data-stu-id="c01a3-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="c01a3-116">В диалоговом окне щелкните **функции почтового ящика**.</span><span class="sxs-lookup"><span data-stu-id="c01a3-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="c01a3-117">В **соответствии с политикой** хранения применяем политику, только что созданную > **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c01a3-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="c01a3-118">Инструкции по применении политики для всех пользователей см. в инструкции применить политику хранения к [почтовым ящикам.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="c01a3-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
