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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232643"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="4a2ea-102">Устранение сообщений, задержанных в папке "Исходящие"</span><span class="sxs-lookup"><span data-stu-id="4a2ea-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="4a2ea-103">Мы рекомендуем начать с выполнения сценария ["проблемы с отправкой, получением или поиском сообщений электронной почты"](https://aka.ms/SaRA-OutlookSendReceive) из центра [поддержки и восстановления Майкрософт](https://diagnostics.office.com/#/) на затронутом компьютере.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="4a2ea-104">Если сообщение застряло в папке "Исходящие", скорее всего, это большое вложение или параметр "отправить сразу после подключения" не включен.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="4a2ea-105">**Удаление большого вложения**</span><span class="sxs-lookup"><span data-stu-id="4a2ea-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="4a2ea-106">Нажмите кнопку **Отправить/получить** > доступ в**автономном режиме**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="4a2ea-107">В области навигации щелкните **папку "Исходящие"**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="4a2ea-108">Отсюда можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="4a2ea-108">From here, you can:</span></span> 
    - <span data-ttu-id="4a2ea-109">Удаление сообщения.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-109">Delete the message.</span></span> <span data-ttu-id="4a2ea-110">Просто выберите его и нажмите кнопку **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="4a2ea-111">Перетащите сообщение в **папку "Черновики"**, дважды щелкните, чтобы открыть сообщение, и удалите вложение (щелкните его и выберите команду **Удалить**).</span><span class="sxs-lookup"><span data-stu-id="4a2ea-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="4a2ea-112">Если сообщение об ошибке указывает, что Outlook пытается передать сообщение, закройте Outlook.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="4a2ea-113">Для выхода может потребоваться несколько секунд.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-113">It may take a few moments to exit.</span></span> <span data-ttu-id="4a2ea-114">Если Outlook не закрывается, нажмите клавиши **CTRL + ALT + DELETE** и выберите **запустить диспетчер задач**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="4a2ea-115">В диспетчере задач перейдите на вкладку **процессы** , прокрутите список до Outlook. exe и нажмите кнопку **завершить процесс**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="4a2ea-116">После закрытия Outlook перезапустите Outlook и повторите шаги 2-3.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="4a2ea-117">После удаления вложения нажмите кнопку **Отправить/получить** > **Автономная работа** , чтобы отменить нажатие кнопки и возобновить работу в сети.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="4a2ea-118">При нажатии кнопки **Отправить**сообщения будут оставаться в папке "Исходящие", но не подключены.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="4a2ea-119">Нажмите кнопку **Отправить/получить** и посмотрите на кнопку **работать в автономном режиме** .</span><span class="sxs-lookup"><span data-stu-id="4a2ea-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="4a2ea-120">Если он синий, то вы отключится.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="4a2ea-121">Щелкните его для подключения (кнопка превращает белый) и нажмите кнопку **отправить все**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="4a2ea-122">**Разрешить немедленную отправку при наличии подключения**</span><span class="sxs-lookup"><span data-stu-id="4a2ea-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="4a2ea-123">На вкладке "Файл" нажмите кнопку **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="4a2ea-124">В диалоговом окне Outlook "Параметры" щелкните **Дополнительно**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="4a2ea-125">В разделе Отправка и получение щелкните, чтобы включить **немедленную отправку при подключении**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="4a2ea-126">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-126">Click **OK**.</span></span>
 
<span data-ttu-id="4a2ea-127">Полные сведения можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="4a2ea-127">For full details, see:</span></span>
- [<span data-ttu-id="4a2ea-128">Видео: отправка и удаление задержанных сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="4a2ea-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="4a2ea-129">Электронная почта остается в папке "Исходящие" до тех пор, пока не будет инициирована операция отправки и получения в Outlook вручную.</span><span class="sxs-lookup"><span data-stu-id="4a2ea-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
