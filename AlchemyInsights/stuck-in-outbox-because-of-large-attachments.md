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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441318"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="11863-102">Устранение сообщений, задержанных в папке "Исходящие"</span><span class="sxs-lookup"><span data-stu-id="11863-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="11863-103">Для начала рекомендуется выполнить сценарий ["проблемы с отправкой, получением или поиском сообщений электронной почты"](https://aka.ms/SaRA-OutlookSendReceive) в средстве [поддержки и восстановления Майкрософт](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="11863-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="11863-104">Когда сообщение зависает в папке "Исходящие", наиболее вероятные причины:</span><span class="sxs-lookup"><span data-stu-id="11863-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="11863-105">Большие вложения.</span><span class="sxs-lookup"><span data-stu-id="11863-105">Large attachments.</span></span>
- <span data-ttu-id="11863-106">Параметр **отправить сразу после подключения** не включен.</span><span class="sxs-lookup"><span data-stu-id="11863-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="11863-107">Удаление больших вложений:</span><span class="sxs-lookup"><span data-stu-id="11863-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="11863-108">В Outlook выберите команду **Отправить и получить** > сведения о**работе в автономном режиме**.</span><span class="sxs-lookup"><span data-stu-id="11863-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="11863-109">В области навигации выберите пункт **Папка "Исходящие"**.</span><span class="sxs-lookup"><span data-stu-id="11863-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="11863-110">Отсюда можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="11863-110">From here, you can:</span></span> 
    - <span data-ttu-id="11863-111">Удалите сообщение (выделите его и нажмите кнопку **Удалить**).</span><span class="sxs-lookup"><span data-stu-id="11863-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="11863-112">Перетащите сообщение в папку "Черновики", дважды щелкните, чтобы открыть его и удалить вложение выберите его и нажмите кнопку **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="11863-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="11863-113">Если появится сообщение об ошибке с сообщением о том, что Outlook пытается передать сообщение, закройте Outlook.</span><span class="sxs-lookup"><span data-stu-id="11863-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="11863-114">Для выхода может потребоваться несколько секунд.</span><span class="sxs-lookup"><span data-stu-id="11863-114">It may take a few moments to exit.</span></span> <span data-ttu-id="11863-115">Если Outlook не закрывается, нажмите клавиши CTRL + ALT + DELETE и выберите пункт **запустить диспетчер задач**.</span><span class="sxs-lookup"><span data-stu-id="11863-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="11863-116">В диспетчере задач перейдите на вкладку **процессы** , прокрутите вниз до Outlook. exe и выберите **завершить процесс**.</span><span class="sxs-lookup"><span data-stu-id="11863-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="11863-117">После закрытия Outlook перезапустите его и повторите шаги 2 и 3.</span><span class="sxs-lookup"><span data-stu-id="11863-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="11863-118">После удаления вложения нажмите кнопку **Отправить/получить** > **Автономная работа** , чтобы возобновить работу в сети.</span><span class="sxs-lookup"><span data-stu-id="11863-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="11863-119">При нажатии кнопки **Отправить**сообщения будут оставаться в папке "Исходящие", но не подключены.</span><span class="sxs-lookup"><span data-stu-id="11863-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="11863-120">Нажмите кнопку **Отправить/получить** и посмотрите на кнопку **работать в автономном режиме** .</span><span class="sxs-lookup"><span data-stu-id="11863-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="11863-121">Если он синий, то вы отключится.</span><span class="sxs-lookup"><span data-stu-id="11863-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="11863-122">Выберите его для подключения (кнопка превращает белый) и нажмите кнопку **отправить все**.</span><span class="sxs-lookup"><span data-stu-id="11863-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="11863-123">Чтобы включить **немедленную отправку при наличии подключения**:</span><span class="sxs-lookup"><span data-stu-id="11863-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="11863-124">Выберите \*\*\*\* > \*\*\*\* >  **Дополнительные**параметры файлов.</span><span class="sxs-lookup"><span data-stu-id="11863-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="11863-125">В разделе **Отправка и получение** нажмите кнопку **отправить сразу же после подключения**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="11863-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="11863-126">Полные сведения можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="11863-126">For full details see:</span></span>
- [<span data-ttu-id="11863-127">Видео: отправка и удаление задержанных сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="11863-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="11863-128">Электронная почта остается в папке "Исходящие" до тех пор, пока не будет инициирована операция отправки и получения в Outlook вручную.</span><span class="sxs-lookup"><span data-stu-id="11863-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
