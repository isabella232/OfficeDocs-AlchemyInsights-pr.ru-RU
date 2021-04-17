---
title: Вход в Windows 10 без использования пароля
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830559"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="94e37-102">Вход в Windows 10 без использования пароля</span><span class="sxs-lookup"><span data-stu-id="94e37-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="94e37-103">Чтобы не вводить пароль при запуске Windows, рекомендуется использовать один из параметров безопасного входного кода Windows Hello, например ПИН-код, распознавание лиц или отпечатки пальцев, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="94e37-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="94e37-104">Если вы действительно хотите отключить безопасный вход, см. ниже инструкции "Автоматически включайся в Windows 10".</span><span class="sxs-lookup"><span data-stu-id="94e37-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="94e37-105">**Безопасные альтернативы Windows Hello для пароля учетной записи**</span><span class="sxs-lookup"><span data-stu-id="94e37-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="94e37-106">Перейдите **к параметрам > учетных записей > параметров** регистрации (или нажмите [здесь).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="94e37-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="94e37-107">Будут перечислены доступные параметры входов.</span><span class="sxs-lookup"><span data-stu-id="94e37-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="94e37-108">Например,</span><span class="sxs-lookup"><span data-stu-id="94e37-108">For example:</span></span>

![Параметры входов.](media/sign-in-options.png)

<span data-ttu-id="94e37-110">Щелкните или нажмите один из параметров, чтобы настроить его.</span><span class="sxs-lookup"><span data-stu-id="94e37-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="94e37-111">При следующем запуске или разблокировать Windows вы сможете использовать новый параметр вместо пароля.</span><span class="sxs-lookup"><span data-stu-id="94e37-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="94e37-112">**Автоматический вход в Windows 10**</span><span class="sxs-lookup"><span data-stu-id="94e37-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="94e37-113">**Примечание.** Автоматическая входная информация удобна, но представляет угрозу безопасности, особенно если компьютер доступен несколькими людьми.</span><span class="sxs-lookup"><span data-stu-id="94e37-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="94e37-114">Щелкните или нажмите **кнопку Начните** в панели задач.</span><span class="sxs-lookup"><span data-stu-id="94e37-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="94e37-115">Введите **netplwiz** и нажмите клавишу Ввод, чтобы открыть окно учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="94e37-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="94e37-116">В **учетных записях** пользователей щелкните учетную запись, включаемую автоматически, в момент начала Windows.</span><span class="sxs-lookup"><span data-stu-id="94e37-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="94e37-117">Отойдите от почтового ящика "Пользователи должны ввести имя пользователя и пароль для использования этого компьютера".</span><span class="sxs-lookup"><span data-stu-id="94e37-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Пользователи должны ввести имя пользователя и пароль.](media/users-must-enter-username.png)

5. <span data-ttu-id="94e37-119">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="94e37-119">Click **OK**.</span></span> <span data-ttu-id="94e37-120">Вам будет предложено ввести и подтвердить пароль выбранной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="94e37-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="94e37-121">Для завершения нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="94e37-121">Click **OK** to finish.</span></span> <span data-ttu-id="94e37-122">При следующем старте Windows 10 она автоматически будет вписываться в выбранную учетную запись.</span><span class="sxs-lookup"><span data-stu-id="94e37-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
