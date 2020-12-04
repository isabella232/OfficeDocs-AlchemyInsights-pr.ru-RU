---
title: Добавление или удаление делегата в Outlook для Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571911"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="c35ab-102">Добавление или удаление делегата в Outlook для Windows</span><span class="sxs-lookup"><span data-stu-id="c35ab-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="c35ab-103">Чтобы добавить делегата в Outlook для Windows, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="c35ab-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="c35ab-104">Перейдите на вкладку **файл** , а затем выберите **Параметры учетной записи**, а затем — **делегированный доступ**.</span><span class="sxs-lookup"><span data-stu-id="c35ab-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="c35ab-105">Нажмите кнопку **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="c35ab-105">Click on **Add**.</span></span> <span data-ttu-id="c35ab-106">Если элемент **Добавить** не отображается, в Outlook и Exchange может не быть активного подключения.</span><span class="sxs-lookup"><span data-stu-id="c35ab-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="c35ab-107">В строке состояния Outlook отображается состояние подключения.</span><span class="sxs-lookup"><span data-stu-id="c35ab-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="c35ab-108">Введите имя человека, которого хотите назначить представителем, или выполните поиск, а затем выберите имя в списке результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="c35ab-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c35ab-109">Представителем должен быть пользователь в глобальном списке адресов Exchange вашей организации (GAL).</span><span class="sxs-lookup"><span data-stu-id="c35ab-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="c35ab-110">Нажмите кнопку **Добавить** , а затем кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="c35ab-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="c35ab-111">В диалоговом окне " **разрешения делегирования** " примите параметры разрешений по умолчанию или выберите Пользовательские уровни доступа для папок Exchange.</span><span class="sxs-lookup"><span data-stu-id="c35ab-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="c35ab-112">Если представителю требуется разрешение для работы только с приглашениями на собрания и ответами, то достаточно изменить параметры разрешений по умолчанию, такие как делегат, на **Получение копий сообщений о собраниях, отправленных мне** .</span><span class="sxs-lookup"><span data-stu-id="c35ab-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="c35ab-113">Параметр разрешения **папки "Входящие"** можно оставить на странице " **нет**".</span><span class="sxs-lookup"><span data-stu-id="c35ab-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="c35ab-114">Приглашения на собрания и ответы будут поступать непосредственно в папку "Входящие" представителя.</span><span class="sxs-lookup"><span data-stu-id="c35ab-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c35ab-115">По умолчанию этому представителю предоставлено разрешение **"редактор" (возможность чтения, создания и изменения элементов)** для папки " **Календарь** ".</span><span class="sxs-lookup"><span data-stu-id="c35ab-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="c35ab-116">Когда представитель отвечает на собрание от вашего имени, он автоматически добавляется в папку " **Календарь** ".</span><span class="sxs-lookup"><span data-stu-id="c35ab-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="c35ab-117">Чтобы отправить сообщение, уведомляющее делегат об измененных разрешениях, установите флажок **автоматически отправлять сообщение для делегирования обобще этих разрешений** .</span><span class="sxs-lookup"><span data-stu-id="c35ab-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="c35ab-118">При необходимости установите флажок **представителю доступны частные элементы** .</span><span class="sxs-lookup"><span data-stu-id="c35ab-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="c35ab-119">Этот параметр влияет на все папки Exchange.</span><span class="sxs-lookup"><span data-stu-id="c35ab-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="c35ab-120">Сюда входят все папки почта, контакты, календарь, задачи, заметки и дневник.</span><span class="sxs-lookup"><span data-stu-id="c35ab-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="c35ab-121">Невозможно предоставить доступ к частным элементам только в указанных папках.</span><span class="sxs-lookup"><span data-stu-id="c35ab-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="c35ab-122">Нажмите кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="c35ab-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="c35ab-123">Сообщения, отправляемые с разрешениями "Отправить от имени", включают в себя **From** и имена, и имена делегата.</span><span class="sxs-lookup"><span data-stu-id="c35ab-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="c35ab-124">Когда сообщение отправляется с разрешениями "Отправить как", отображается только ваше имя.</span><span class="sxs-lookup"><span data-stu-id="c35ab-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="c35ab-125">Когда вы добавляете кого-либо представителем, он может добавить свой почтовый ящик Exchange в свой профиль Outlook.</span><span class="sxs-lookup"><span data-stu-id="c35ab-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="c35ab-126">Инструкции: Manage a [mail and Calendar Items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="c35ab-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="c35ab-127">Чтобы удалить делегата в Outlook для Windows, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="c35ab-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="c35ab-128">Перейдите на вкладку **файл** .</span><span class="sxs-lookup"><span data-stu-id="c35ab-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="c35ab-129">Щелкните **Параметры учетной записи** , а затем — **делегированный доступ**.</span><span class="sxs-lookup"><span data-stu-id="c35ab-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="c35ab-130">Выберите имя представителя, для которого необходимо изменить разрешения, а затем нажмите кнопку **Удалить** , а затем **ОК**.</span><span class="sxs-lookup"><span data-stu-id="c35ab-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
