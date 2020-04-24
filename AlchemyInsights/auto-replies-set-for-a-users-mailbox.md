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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788895"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="9eb78-102">Настройка автоматических ответов для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="9eb78-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="9eb78-103">**Метод 1**</span><span class="sxs-lookup"><span data-stu-id="9eb78-103">**Method 1**</span></span>

1. <span data-ttu-id="9eb78-104">Войдите на портал Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9eb78-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="9eb78-105">Выберите **Пользователи > Активные пользователи** (или **Группы > Общие почтовые ящики**, если выполняется настройка в общем почтовом ящике).</span><span class="sxs-lookup"><span data-stu-id="9eb78-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="9eb78-106">Выберите пользователя, у которого есть почтовый ящик Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="9eb78-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="9eb78-107">Во всплывающем меню справа выберите **Параметры почты > Автоматические ответы** (если это общий почтовый ящик, просто щелкните **Автоматические ответы** во всплывающем меню).</span><span class="sxs-lookup"><span data-stu-id="9eb78-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="9eb78-108">**Метод 2**</span><span class="sxs-lookup"><span data-stu-id="9eb78-108">**Method 2**</span></span>

1. <span data-ttu-id="9eb78-109">Войдите на портал администрирования Microsoft 365, используя учетные данные администратора.</span><span class="sxs-lookup"><span data-stu-id="9eb78-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="9eb78-110">Разверните пункт **Центры администрирования** и щелкните **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9eb78-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="9eb78-111">Щелкните изображение в правом верхнем углу, нажмите **Еще один пользователь** и выберите почтовый ящик пользователя, который нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="9eb78-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="9eb78-112">В левой части выберите **Параметры**, щелкните **Упорядочить электронную почту** и нажмите **Автоматические ответы**.</span><span class="sxs-lookup"><span data-stu-id="9eb78-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="9eb78-113">**Метод 3**</span><span class="sxs-lookup"><span data-stu-id="9eb78-113">**Method 3**</span></span>

<span data-ttu-id="9eb78-114">В Exchange Online PowerShell выполните следующий командлет:</span><span class="sxs-lookup"><span data-stu-id="9eb78-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="9eb78-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="9eb78-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="9eb78-116">Дополнительные сведения об этом командлете см. в статье [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="9eb78-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
