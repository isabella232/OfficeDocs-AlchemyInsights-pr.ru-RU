---
title: Автоматическое шифрование определенных сообщений электронной почты Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510214"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="996f9-102">Автоматическое шифрование определенных сообщений электронной почты Office 365</span><span class="sxs-lookup"><span data-stu-id="996f9-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="996f9-103">Вы можете автоматически шифровать сообщения, которые пользователи отправляют определенным внешним людям или организациям.</span><span class="sxs-lookup"><span data-stu-id="996f9-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="996f9-104">Для этого выполните описанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="996f9-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="996f9-105">В центре [администрирования Exchange](https://outlook.office365.com/ecp/)выберите поток **почты > правила.**</span><span class="sxs-lookup"><span data-stu-id="996f9-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="996f9-106">Щелкните **значок New (+)** и нажмите кнопку **Применить шифрование сообщений Office 365** и защиту прав на сообщения.</span><span class="sxs-lookup"><span data-stu-id="996f9-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="996f9-107">В **Name** введите имя правила, например шифруем сообщений, отправленных *в DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="996f9-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="996f9-108">В **Применение этого правила,** если , выберите **получатель > это лицо**.</span><span class="sxs-lookup"><span data-stu-id="996f9-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="996f9-109">В окне **Select Members** выберите имя человека, к которого необходимо применить правило шифрования, а затем нажмите **кнопку добавить**.</span><span class="sxs-lookup"><span data-stu-id="996f9-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="996f9-110">После добавления пользователей нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="996f9-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="996f9-111">Рядом со следующим **полем Do** щелкните **Выберите одно.**</span><span class="sxs-lookup"><span data-stu-id="996f9-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="996f9-112">В **выпадаемом меню** шаблона RMS выберите **Шифруй** и нажмите **кнопку ОК.**</span><span class="sxs-lookup"><span data-stu-id="996f9-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="996f9-113">(Если вы не видите этот параметр, это означает, что ваш план не включает автоматическое шифрование.</span><span class="sxs-lookup"><span data-stu-id="996f9-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="996f9-114">Но вы можете добавить его!)</span><span class="sxs-lookup"><span data-stu-id="996f9-114">But you can add it!)</span></span>
9. <span data-ttu-id="996f9-115">Выберите любой необязательный выбор (из списка необязательных выборов, которые можно сделать на данном этапе, многие из которых можно оставить с параметром по умолчанию для простоты).</span><span class="sxs-lookup"><span data-stu-id="996f9-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="996f9-116">Щелкните **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="996f9-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="996f9-117">Вы всегда можете вернуться и изменить это правило позже.</span><span class="sxs-lookup"><span data-stu-id="996f9-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="996f9-118">Дополнительные сведения о создании правил шифрования см. в тексте Определение правил потока почты для шифрования сообщений электронной почты [в Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="996f9-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

