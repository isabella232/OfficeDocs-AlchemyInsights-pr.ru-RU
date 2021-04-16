---
title: Открыть файл только для чтения
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813197"
---
# <a name="file-open-read-only"></a><span data-ttu-id="ba4c4-102">Открыть файл только для чтения</span><span class="sxs-lookup"><span data-stu-id="ba4c4-102">File open read-only</span></span>

<span data-ttu-id="ba4c4-103">Вы можете обнаружить, что при открытии файлов они открываются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="ba4c4-104">В некоторых случаях это для добавленной безопасности, например при открытии файлов из Интернета, а в других случаях это может быть связано с параметром, который можно изменить.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="ba4c4-105">Вот некоторые сценарии, в которых файл открывается только для чтения, и некоторые действия, которые можно предпринять, чтобы изменить это.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="ba4c4-106">**Мой антивирус вызывает их, чтобы открыть только для чтения**</span><span class="sxs-lookup"><span data-stu-id="ba4c4-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="ba4c4-107">Некоторые антивирусные программы могут защитить вас от потенциально небезопасных файлов, открыв их только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="ba4c4-108">Возможно, вам потребуется проверить у поставщика антивирусов, чтобы узнать, как настроить эти параметры.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="ba4c4-109">BitDefender, например, имеет контент по добавлению исключений приложений здесь: Как добавить исключения приложений или процессов в Центре управления [Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="ba4c4-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="ba4c4-110">**Настроены ли свойства файла только для чтения?**</span><span class="sxs-lookup"><span data-stu-id="ba4c4-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="ba4c4-111">Вы можете проверить свойства файла, щелкнув правой кнопкой мыши по файлу и выбрав свойства.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="ba4c4-112">Если атрибут только для чтения проверяется, его можно отойдите и нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="ba4c4-113">**Содержимое находится в защищенной области зрения**</span><span class="sxs-lookup"><span data-stu-id="ba4c4-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="ba4c4-114">Файлы из Интернета и из других потенциально небезопасных местоположений могут содержать вирусы, черви или другие виды вредоносных программ, которые могут нанести вред компьютеру.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="ba4c4-115">Это также часто встречается с вложениями электронной почты или файлами, которые вы скачали.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="ba4c4-116">Чтобы защитить компьютер, файлы из этих потенциально небезопасных местоположений открываются в защищенной папке View.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="ba4c4-117">С помощью protected View можно читать файл и просматривать его содержимое, снижая риски.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="ba4c4-118">Дополнительные сведения о защищенных представлениях и изменениях параметров см. в этой статье: [Что такое защищенный вид?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="ba4c4-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="ba4c4-119">**Заполнен ли OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="ba4c4-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="ba4c4-120">Если файл хранится в OneDrive, а пространство хранения OneDrive заполнено, сохранить документ будет невозможно, пока он не будет выделен.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="ba4c4-121">Вы можете проверить свободное пространство в OneDrive, щелкнув значок OneDrive в центре уведомлений и выбрав управление хранилищем, или вы можете перейти к входу и отметить количество используемого пространства в нижней левой части [https://onedrive.live.com](https://onedrive.live.com) экрана.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="ba4c4-122">**Активируется ли Office?**</span><span class="sxs-lookup"><span data-stu-id="ba4c4-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="ba4c4-123">Если Office не активирован или срок действия подписки истек, вы можете быть в режиме "Уменьшенная функциональность" только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="ba4c4-124">Сведения о том, как активировать Office, см. в руб. Ошибки без лицензии на продукт и [активацию в Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="ba4c4-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="ba4c4-125">**Если все остальное не удается ...**</span><span class="sxs-lookup"><span data-stu-id="ba4c4-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="ba4c4-126">Попробуйте перезапустить компьютер</span><span class="sxs-lookup"><span data-stu-id="ba4c4-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="ba4c4-127">Установка обновлений Office</span><span class="sxs-lookup"><span data-stu-id="ba4c4-127">Install Office updates</span></span>
    
- <span data-ttu-id="ba4c4-128">Выполнение ремонта Office в Интернете</span><span class="sxs-lookup"><span data-stu-id="ba4c4-128">Perform an Online repair of Office</span></span>
    

