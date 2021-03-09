---
title: Отправка сообщения электронной почты путем предоставления сетевого ИД сообщения
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552355"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="5b5d5-102">Отправка сообщения электронной почты путем предоставления сетевого ИД сообщения</span><span class="sxs-lookup"><span data-stu-id="5b5d5-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="5b5d5-103">В новой **вылетной записи** отправки выберите **ID электронной** почты и **сетевого сообщения.**</span><span class="sxs-lookup"><span data-stu-id="5b5d5-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="5b5d5-104">Выполните следующие действия, чтобы найти ID сообщения для сообщения электронной почты в Outlook:</span><span class="sxs-lookup"><span data-stu-id="5b5d5-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="5b5d5-105">Дважды щелкните сообщение электронной почты, чтобы открыть его.</span><span class="sxs-lookup"><span data-stu-id="5b5d5-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="5b5d5-106">Выберите **свойства**  >  **файлов**.</span><span class="sxs-lookup"><span data-stu-id="5b5d5-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="5b5d5-107">Откройте блокнот или пустой документ Word, а затем скопируйте  и вклейте содержимое, найденное в поле загонщиков Интернета, в открытый документ для лучшей видимости.</span><span class="sxs-lookup"><span data-stu-id="5b5d5-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="5b5d5-108">Найдите **поле X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="5b5d5-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="5b5d5-109">Значение после **:** — это ID, необходимый для отправки.</span><span class="sxs-lookup"><span data-stu-id="5b5d5-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="5b5d5-110">В **соответствии с получателями,** если электронная почта приземлилась в папке нежелательной почты для всех получателей этой электронной почты, выберите **Выберите Все**.</span><span class="sxs-lookup"><span data-stu-id="5b5d5-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="5b5d5-111">Если нет, выберите только пользователя, который сообщил о проблеме.</span><span class="sxs-lookup"><span data-stu-id="5b5d5-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="5b5d5-112">В **статье Причина** отправки, если выбрано, должно быть заблокировано, укажите, должно ли сообщение быть заблокировано как спам, **фишинг** или вредоносные **программы,** а затем выберите **Отправить**.  </span><span class="sxs-lookup"><span data-stu-id="5b5d5-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="5b5d5-113">Дополнительные данные см. в материалах [How to submit suspected spam, phish, URLs and files to Microsoft for scanning.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="5b5d5-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
