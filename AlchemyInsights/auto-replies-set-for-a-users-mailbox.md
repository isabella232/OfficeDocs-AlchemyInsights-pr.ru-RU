---
title: Настройка автоматических ответов для почтового ящика
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715142"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="1acde-102">Настройка автоматических ответов для почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="1acde-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="1acde-103">**Метод 1**</span><span class="sxs-lookup"><span data-stu-id="1acde-103">**Method 1**</span></span>

1. <span data-ttu-id="1acde-104">Войдите на портал Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1acde-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="1acde-105">Выберите **Пользователи > Активные пользователи** (или **Группы > Общие почтовые ящики**, если выполняется настройка в общем почтовом ящике).</span><span class="sxs-lookup"><span data-stu-id="1acde-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="1acde-106">Выберите пользователя, у которого есть почтовый ящик Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="1acde-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="1acde-107">Во всплывающем меню справа выберите **Параметры почты > Автоматические ответы** (если это общий почтовый ящик, просто щелкните **Автоматические ответы** во всплывающем меню).</span><span class="sxs-lookup"><span data-stu-id="1acde-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="1acde-108">**Метод 2**</span><span class="sxs-lookup"><span data-stu-id="1acde-108">**Method 2**</span></span>

1. <span data-ttu-id="1acde-109">Войдите на портал администрирования Microsoft 365, используя учетные данные администратора.</span><span class="sxs-lookup"><span data-stu-id="1acde-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="1acde-110">Разверните пункт **Центры администрирования** и щелкните **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1acde-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="1acde-111">Щелкните изображение в правом верхнем углу, нажмите **Еще один пользователь** и выберите почтовый ящик пользователя, который нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="1acde-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="1acde-112">В левой части выберите **Параметры**, щелкните **Упорядочить электронную почту** и нажмите **Автоматические ответы**.</span><span class="sxs-lookup"><span data-stu-id="1acde-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="1acde-113">**Метод 3**</span><span class="sxs-lookup"><span data-stu-id="1acde-113">**Method 3**</span></span>

<span data-ttu-id="1acde-114">В Exchange Online PowerShell выполните следующий командлет:</span><span class="sxs-lookup"><span data-stu-id="1acde-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="1acde-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="1acde-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="1acde-116">Дополнительные сведения об этом командлете см. в статье [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="1acde-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
