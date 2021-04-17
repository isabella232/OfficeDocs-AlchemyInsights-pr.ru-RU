---
title: Настройка автоматических ответов для почтового ящика
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820947"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="52d8a-102">Настройка автоматических ответов для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="52d8a-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="52d8a-103">**Метод 1**</span><span class="sxs-lookup"><span data-stu-id="52d8a-103">**Method 1**</span></span>

1. <span data-ttu-id="52d8a-104">Войдите на портал Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52d8a-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="52d8a-105">Выберите **Пользователи > Активные пользователи** (или **Группы > Общие почтовые ящики**, если выполняется настройка в общем почтовом ящике).</span><span class="sxs-lookup"><span data-stu-id="52d8a-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="52d8a-106">Выберите пользователя, у которого есть почтовый ящик Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="52d8a-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="52d8a-107">Во всплывающем меню справа выберите **Параметры почты > Автоматические ответы** (если это общий почтовый ящик, просто щелкните **Автоматические ответы** во всплывающем меню).</span><span class="sxs-lookup"><span data-stu-id="52d8a-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="52d8a-108">**Метод 2**</span><span class="sxs-lookup"><span data-stu-id="52d8a-108">**Method 2**</span></span>

1. <span data-ttu-id="52d8a-109">Войдите на портал администрирования Microsoft 365, используя учетные данные администратора.</span><span class="sxs-lookup"><span data-stu-id="52d8a-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="52d8a-110">Разверните пункт **Центры администрирования** и щелкните **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="52d8a-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="52d8a-111">Щелкните изображение в правом верхнем углу, нажмите **Еще один пользователь** и выберите почтовый ящик пользователя, который нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="52d8a-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="52d8a-112">В левой части выберите **Параметры**, щелкните **Упорядочить электронную почту** и нажмите **Автоматические ответы**.</span><span class="sxs-lookup"><span data-stu-id="52d8a-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="52d8a-113">**Метод 3**</span><span class="sxs-lookup"><span data-stu-id="52d8a-113">**Method 3**</span></span>

<span data-ttu-id="52d8a-114">В Exchange Online PowerShell выполните следующий командлет:</span><span class="sxs-lookup"><span data-stu-id="52d8a-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="52d8a-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="52d8a-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="52d8a-116">Дополнительные сведения об этом командлете см. в статье [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="52d8a-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
