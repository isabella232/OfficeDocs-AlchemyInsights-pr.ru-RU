---
title: Задержано в папке "Исходящие" из-за больших вложений
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241265"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="328b3-102">Устранение сообщений, задержанных в папке "Исходящие"</span><span class="sxs-lookup"><span data-stu-id="328b3-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="328b3-103">Для начала рекомендуется выполнить сценарий ["проблемы с отправкой, получением или поиском сообщений электронной почты"](https://aka.ms/SaRA-OutlookSendReceive) в средстве [поддержки и восстановления Майкрософт](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="328b3-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="328b3-104">Если сообщение застряло в папке "Исходящие", скорее всего, это большое вложение или параметр "отправить сразу после подключения" не включен.</span><span class="sxs-lookup"><span data-stu-id="328b3-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="328b3-105">**Удаление большого вложения**</span><span class="sxs-lookup"><span data-stu-id="328b3-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="328b3-106">В Outlook выберите команду **Отправить и получить** > сведения о**работе в автономном режиме**.</span><span class="sxs-lookup"><span data-stu-id="328b3-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="328b3-107">В области навигации выберите пункт **Папка "Исходящие"**.</span><span class="sxs-lookup"><span data-stu-id="328b3-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="328b3-108">Отсюда можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="328b3-108">From here, you can:</span></span> 
    - <span data-ttu-id="328b3-109">Удалите сообщение (выделите его и нажмите кнопку **Удалить**).</span><span class="sxs-lookup"><span data-stu-id="328b3-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="328b3-110">Перетащите сообщение в папку "Черновики", дважды щелкните, чтобы открыть его и удалить вложение выберите его и нажмите кнопку **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="328b3-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="328b3-111">Если появится сообщение об ошибке с сообщением о том, что Outlook пытается передать сообщение, закройте Outlook.</span><span class="sxs-lookup"><span data-stu-id="328b3-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="328b3-112">Для выхода может потребоваться несколько секунд.</span><span class="sxs-lookup"><span data-stu-id="328b3-112">It may take a few moments to exit.</span></span> <span data-ttu-id="328b3-113">Если Outlook не закрывается, нажмите клавиши CTRL + ALT + DELETE и выберите пункт **запустить диспетчер задач**.</span><span class="sxs-lookup"><span data-stu-id="328b3-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="328b3-114">В диспетчере задач перейдите на вкладку **процессы** , прокрутите вниз до Outlook. exe и выберите **завершить процесс**.</span><span class="sxs-lookup"><span data-stu-id="328b3-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="328b3-115">После закрытия Outlook перезапустите его и повторите шаги 2 и 3.</span><span class="sxs-lookup"><span data-stu-id="328b3-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="328b3-116">После удаления вложения нажмите кнопку **Отправить/получить** > **Автономная работа** , чтобы возобновить работу в сети.</span><span class="sxs-lookup"><span data-stu-id="328b3-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="328b3-117">При нажатии кнопки **Отправить**сообщения будут оставаться в папке "Исходящие", но не подключены.</span><span class="sxs-lookup"><span data-stu-id="328b3-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="328b3-118">Нажмите кнопку **Отправить/получить** и посмотрите на кнопку **работать в автономном режиме** .</span><span class="sxs-lookup"><span data-stu-id="328b3-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="328b3-119">Если он синий, то вы отключится.</span><span class="sxs-lookup"><span data-stu-id="328b3-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="328b3-120">Щелкните его для подключения (кнопка превращает белый) и нажмите кнопку **отправить все**.</span><span class="sxs-lookup"><span data-stu-id="328b3-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="328b3-121">**Разрешить немедленную отправку при наличии подключения**</span><span class="sxs-lookup"><span data-stu-id="328b3-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="328b3-122">На вкладке "Файл" нажмите кнопку **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="328b3-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="328b3-123">В диалоговом окне Outlook "Параметры" щелкните **Дополнительно**.</span><span class="sxs-lookup"><span data-stu-id="328b3-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="328b3-124">В разделе Отправка и получение щелкните, чтобы включить **немедленную отправку при подключении**.</span><span class="sxs-lookup"><span data-stu-id="328b3-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="328b3-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="328b3-125">Click **OK**.</span></span>
 
<span data-ttu-id="328b3-126">Полные сведения можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="328b3-126">For full details, see:</span></span>
- [<span data-ttu-id="328b3-127">Видео: отправка и удаление задержанных сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="328b3-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="328b3-128">Электронная почта остается в папке "Исходящие" до тех пор, пока не будет инициирована операция отправки и получения в Outlook вручную.</span><span class="sxs-lookup"><span data-stu-id="328b3-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
