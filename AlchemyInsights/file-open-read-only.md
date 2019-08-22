---
title: Файл открыт только для чтения
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 5c28d5f1c6951971aab329060e24b8458e848dd7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525684"
---
# <a name="file-open-read-only"></a><span data-ttu-id="6f308-102">Файл открыт только для чтения</span><span class="sxs-lookup"><span data-stu-id="6f308-102">File open read-only</span></span>

<span data-ttu-id="6f308-103">Если вы открываете файлы, они могут открываться только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f308-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="6f308-104">В некоторых случаях это относится к дополнительным системам безопасности, например, при открытии файлов из Интернета и в других случаях может быть вызвана изменяемым параметром.</span><span class="sxs-lookup"><span data-stu-id="6f308-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="6f308-105">Ниже приведено несколько сценариев, в которых файл открывается только для чтения, и можно выполнить некоторые действия, чтобы изменить его.</span><span class="sxs-lookup"><span data-stu-id="6f308-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="6f308-106">**Антивирусная программа вызывает открытие только для чтения**</span><span class="sxs-lookup"><span data-stu-id="6f308-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="6f308-107">Некоторые антивирусные программы могут защитить вас от потенциально небезопасных файлов, открыв их только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f308-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="6f308-108">Чтобы узнать, как настроить эти параметры, обратитесь к поставщику антивирусной программы.</span><span class="sxs-lookup"><span data-stu-id="6f308-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="6f308-109">Битдефендер, например, содержит сведения о добавлении исключений приложений здесь: [как добавить исключения приложений или процессов в центр управления битдефендер](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="6f308-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="6f308-110">**Свойства файлов задаются только для чтения?**</span><span class="sxs-lookup"><span data-stu-id="6f308-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="6f308-111">Чтобы проверить свойства файла, щелкните его правой кнопкой мыши и выберите пункт Свойства.</span><span class="sxs-lookup"><span data-stu-id="6f308-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="6f308-112">Если установлен флажок атрибут только для чтения, его можно снять и нажать кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="6f308-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="6f308-113">**Содержимое находится в режиме защищенного просмотра**</span><span class="sxs-lookup"><span data-stu-id="6f308-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="6f308-114">Файлы из Интернета и других потенциально небезопасных расположений могут содержать вирусы, черви или другие вредоносные программы, которые могут повредить компьютер.</span><span class="sxs-lookup"><span data-stu-id="6f308-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="6f308-115">Обычно это происходит с вложениями электронной почты или скачанными файлами.</span><span class="sxs-lookup"><span data-stu-id="6f308-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="6f308-116">В целях защиты компьютера файлы из этих потенциально небезопасных расположений открываются в режиме защищенного просмотра.</span><span class="sxs-lookup"><span data-stu-id="6f308-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="6f308-117">С помощью режима защищенного просмотра можно читать файл и просматривать его содержимое, а также сокращать риски.</span><span class="sxs-lookup"><span data-stu-id="6f308-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="6f308-118">Дополнительные сведения о режиме защищенного просмотра и о том, как изменить параметры, приведены в этой статье: [что такое защищенный просмотр?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="6f308-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="6f308-119">**Является заполнением OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="6f308-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="6f308-120">Если файл хранится в OneDrive, а пространство для хранения OneDrive заполнено, вы не сможете сохранить документ до тех пор, пока вы не освободите отведенный вам объем.</span><span class="sxs-lookup"><span data-stu-id="6f308-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="6f308-121">Чтобы проверить свободное место в OneDrive, щелкните значок OneDrive в центре уведомлений и выберите Управление хранилищем [http://onedrive.live.com](http://onedrive.live.com), а затем войдите в систему и запишите объем занятого места в левом нижнем углу экрана.</span><span class="sxs-lookup"><span data-stu-id="6f308-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="6f308-122">**Активирован ли Office?**</span><span class="sxs-lookup"><span data-stu-id="6f308-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="6f308-123">Если Office не активирован или срок действия подписки истек, можно использовать режим ограниченной функциональности "только для чтения".</span><span class="sxs-lookup"><span data-stu-id="6f308-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="6f308-124">Сведения о том, как активировать Office, приведены в статье: нелицензированные [продукты и ошибки активации в Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="6f308-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="6f308-125">**Если ничего не происходит...**</span><span class="sxs-lookup"><span data-stu-id="6f308-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="6f308-126">Попробуйте перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="6f308-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="6f308-127">Установка обновлений Office</span><span class="sxs-lookup"><span data-stu-id="6f308-127">Install Office updates</span></span>
    
- <span data-ttu-id="6f308-128">Выполнение оперативного восстановления Office</span><span class="sxs-lookup"><span data-stu-id="6f308-128">Perform an Online repair of Office</span></span>
    

