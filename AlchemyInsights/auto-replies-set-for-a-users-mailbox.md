---
title: Настройка автоматических ответов для почтового ящика
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509514"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="a606e-102">Настройка автоматических ответов для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="a606e-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="a606e-103">**Метод 1**</span><span class="sxs-lookup"><span data-stu-id="a606e-103">**Method 1**</span></span>

1. <span data-ttu-id="a606e-104">Войдите на портал Office 365.</span><span class="sxs-lookup"><span data-stu-id="a606e-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="a606e-105">Выберите **Пользователи > Активные пользователи** (или **Группы > Общие почтовые ящики**, если выполняется настройка в общем почтовом ящике).</span><span class="sxs-lookup"><span data-stu-id="a606e-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="a606e-106">Выберите пользователя, у которого есть почтовый ящик Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="a606e-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="a606e-107">Во всплывающем меню справа выберите **Параметры почты > Автоматические ответы** (если это общий почтовый ящик, просто щелкните **Автоматические ответы** во всплывающем меню).</span><span class="sxs-lookup"><span data-stu-id="a606e-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="a606e-108">**Метод 2**</span><span class="sxs-lookup"><span data-stu-id="a606e-108">**Method 2**</span></span>

1. <span data-ttu-id="a606e-109">Войдите на портал администрирования Office 365, используя учетные данные администратора.</span><span class="sxs-lookup"><span data-stu-id="a606e-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="a606e-110">Разверните пункт **Центры администрирования** и щелкните **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="a606e-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="a606e-111">Щелкните изображение в правом верхнем углу, нажмите **Еще один пользователь** и выберите почтовый ящик пользователя, который нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="a606e-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="a606e-112">В левой части выберите **Параметры**, щелкните **Упорядочить электронную почту** и нажмите **Автоматические ответы**.</span><span class="sxs-lookup"><span data-stu-id="a606e-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="a606e-113">**Метод 3**</span><span class="sxs-lookup"><span data-stu-id="a606e-113">**Method 3**</span></span>

<span data-ttu-id="a606e-114">В Exchange Online PowerShell выполните следующий командлет:</span><span class="sxs-lookup"><span data-stu-id="a606e-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="a606e-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a606e-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="a606e-116">Дополнительные сведения об этом командлете см. в статье [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="a606e-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
